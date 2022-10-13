# Infrastructure
Infrastructure as Code with CloudFormation

To create stack run the below command in AWS CLI:
'''aws cloudformation create-stack  \
 --stack-name myteststack1   --template-body file://vpc1.yml \
 --parameters ParameterKey=VpcCIDR,ParameterValue="10.0.0.0/16" ParameterKey=PublicSubnet1CIDR,ParameterValue="10.0.3.0/24" ParameterKey=PublicSubnet2CIDR,ParameterValue="10.0.4.0/24" ParameterKey=PublicSubnet3CIDR,ParameterValue="10.0.5.0/24"  --profile Dev_Admin --region us-east-1'''

To delete stack run the below command in AWS CLI:

'''aws cloudformation delete-stack --stack-name myteststack1 --profile Dev_Admin --region us-west-1'''

check the status of stack in AWS console. 

