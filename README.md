crear cloud9 ... asignar role cloud9fulladmin

acceder

```
cd /home/ubuntu/.ssh

cat > /home/ubuntu/.ssh/id_rsa.imp << 'EOF'
-----BEGIN OPENSSH PRIVATE KEY-----
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
-----END OPENSSH PRIVATE KEY-----
EOF

cat > /home/ubuntu/.ssh/id_rsa.pub.imp << 'EOF'
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCOsaTdr9qc1WFJK7H5/sHpH8oRTMlqRZwb5XDn3Lp2EPOsb9wiYiZNvtGTPFqy4miY9KgZzQ3/vQVdU6GWria8D4UIMfKANFNa/byFc4zIXPGALLYl7hhB/MHx6UPKu+twqgtN52qbmPwfIqgwcMOt2s3I3Qd2FGf3Nn6jgFGhlZhhmZUI3DiEe0E35jbUYbUCBoAmFKQNlvLFrKxJ54lhAbbZY/pEh0X07SbO18JVJMYjdsxtruqlf6AcnNQornlNqwssb80xzaS8+irJlc9ykjUOEtVx/u4E3w93JR05ETBUOQxD1fLQYM2DK6EbMw9Xzx9ICEIo07J9wm4tkBw8RXC+CRUoUzo9nsqeXFQIdN8BwSiZfQE6GJxd84aHCd0nLjCfwwdzOcJJblCRPYdko87S7aStOA3lPU64cmahCpFkQhDfo/EXWyGO/ph7+nT02P0RmajqEj55On8C/h3eC5b0yYquMU8lyJ8JrhtHIAuiz30JHlizHTheCY2x2Sk= ubuntu@ip-172-31-1-153
EOF

chmod 500 /home/ubuntu/.ssh/id_rsa.priv
mv -f /home/ubuntu/.ssh/id_rsa.imp /home/ubuntu/.ssh/id_rsa
mv -f /home/ubuntu/.ssh/id_rsa.pub.imp /home/ubuntu/.ssh/id_rsa.pub
```

#clonar repo
```
cd  /home/ubuntu/environment
git clone git@github.com:speedyrails/workshop-2024-09.git
```
crear  vpc
```
aws cloudformation create-stack --stack-name workshop --template-body file://01-cfn-vpc.yaml 
```
crear eks en redes
```
curl --silent --location "https://github.com/weaveworks/eksctl/releases/download/v0.114.0/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
sudo mv /tmp/eksctl /usr/local/bin

curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.21.2/2021-07-05/bin/linux/amd64/kubectl
chmod +x ./kubectl
sudo mv ./kubectl /usr/local/bin
```

crear el cluster
```
CLUSTER_NAME=workshop
PUBLIC_SUBNET=`aws cloudformation describe-stacks --stack-name workshop  --query "Stacks[0].Outputs[?OutputKey=='PublicSubnets'].OutputValue" --output text`
PRIVATE_SUBNET=`aws cloudformation describe-stacks --stack-name workshop  --query "Stacks[0].Outputs[?OutputKey=='PrivateSubnets'].OutputValue" --output text`
REGION=`curl http://169.254.169.254/latest/meta-data/placement/region`        

eksctl create cluster --name ${CLUSTER_NAME}  \
      --timeout 20m \
      --version 1.23 \
      --region ${REGION} \
       --with-oidc \
      --without-nodegroup \
      --authenticator-role-arn string  \
      --vpc-public-subnets=${PUBLIC_SUBNET} \
      --vpc-private-subnets=${PRIVATE_SUBNET}

aws eks update-kubeconfig --name ${CLUSTER_NAME}


eksctl create nodegroup \
  --cluster ${CLUSTER_NAME} \
  --region ${REGION} \
  --name ng-1 \
  --node-type t3.medium \
  --nodes-min 1 \
  --nodes-max 3 \
  --node-volume-size 40 \
  --managed

eksctl create addon --name coredns --cluster ${CLUSTER_NAME} --region ${REGION} --force
eksctl create addon --name kube-proxy --cluster ${CLUSTER_NAME} --region ${REGION} --force
eksctl create addon --name vpc-cni --cluster ${CLUSTER_NAME} --region ${REGION} --force

```

Instalacion de una aplicacion de ejemplo

ALB_VERSION=v2.2.0
ALB_VERSION_FILE=v2_2_0_full

curl -o iam-policy.json https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/${ALB_VERSION}/docs/install/iam_policy.json

aws iam create-policy \
    --policy-name EKS-AWSLoadBalancerControllerIAMPolicy-${CLUSTER_NAME} \
    --policy-document file://iam-policy.json
        
eksctl create iamserviceaccount \
--cluster=${CLUSTER_NAME} \
--region=${REGION} \
--namespace=kube-system \
--name=aws-load-balancer-controller \
--attach-policy-arn=arn:aws:iam::$USER_ID:policy/EKS-AWSLoadBalancerControllerIAMPolicy-${CLUSTER_NAME} \
--override-existing-serviceaccounts \
--approve







Proceso de actualizacion y correccion

Los nodos estan en una red publica .. pasarlo a una privada
OrganizationAccountAccessRole:~ $ kubectl get nodes -o wide
NAME                         STATUS   ROLES    AGE   VERSION                INTERNAL-IP   EXTERNAL-IP    OS-IMAGE         KERNEL-VERSION                  CONTAINER-RUNTIME
ip-10-0-59-40.ec2.internal   Ready    <none>   19m   v1.23.17-eks-1552ad0   10.0.59.40    98.81.234.16   Amazon Linux 2   5.10.223-212.873.amzn2.x86_64   docker://25.0.6


Para pasarlos a una privada se crea un nodegroup nuevo

eksctl create nodegroup \
  --cluster ${CLUSTER_NAME} \
  --region ${REGION} \
  --name ng-3 \
  --node-type t3.medium \
  --nodes-min 1 \
  --nodes-max 3 \
  --node-volume-size 40 \
  --managed \
  --node-private-networking
  

Actualizacion del ALB

Karpenter or AWS Autoscaler


CloudWatch ?
Problemas de costos si karpenter crear nodos frecuentemente


      
      

  
