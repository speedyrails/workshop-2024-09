crear cloud9 ... asignar role cloud9fulladmin

acceder 

clonar repo 

crear  vpc
aws cloudformation create-stack --stack-name myteststack --template-body file://01-cfn-vpc.yaml 

crear eks en redes
curl --silent --location "https://github.com/weaveworks/eksctl/releases/download/v0.114.0/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
mv /tmp/eksctl /usr/local/bin


crear el cluster
CLUSTER_NAME=workshop
PUBLIC_SUBNET=`aws cloudformation describe-stacks --stack-name myteststack  --query "Stacks[0].Outputs[?OutputKey=='PublicSubnets'].OutputValue" --output text`
REGION=$(aws configure get region)

eksctl create cluster --name ${CLUSTER_NAME}  \
      --timeout 20m \
      --version 1.23 \
       --with-oidc \
      --without-nodegroup \
      --authenticator-role-arn string  \
      --vpc-public-subnets=${PUBLIC_SUBNET}


eksctl create nodegroup \
  --cluster ${CLUSTER_NAME} \
  --region ${REGION} \
  --name ng-1 \
  --instance-types t3.medium \
  --desired-capacity 2 \
  --min-size 1 \
  --max-size 3 \
  --volume-size 20 \
  --managed
  
