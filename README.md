crear cloud9
clonar repo

crear  vpc
aws cloudformation create-stack --stack-name myteststack --template-body file://01-cfn-vpc.yaml 

crear eks en redes
curl --silent --location "https://github.com/weaveworks/eksctl/releases/download/v0.114.0/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
mv /tmp/eksctl /usr/local/bin

PUBLIC_SUBNET=`aws cloudformation describe-stacks --stack-name myteststack  --query "Stacks[0].Outputs[?OutputKey=='PublicSubnets'].OutputValue" --output text`

echo eksctl create cluster --name workshoop  \
      --timeout 20m \
      --version 1.23 \
       --with-oidc \
      --without-nodegroup \
      --authenticator-role-arn string  \
      --vpc-public-subnets=${PUBLIC_SUBNET}




