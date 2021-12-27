# AWS-EC2-Boto3-and-Python
AWS Boto3 is the Python SDK for AWS. Boto3 can be used to directly interact with AWS resources from Python scripts. 

```

import boto3
ec2 = boto3.resource('ec2')

# create a new EC2 instance
instances = ec2.create_instances(
     ImageId='ami-00b6a8a2bd28daf19',
     MinCount=1,
     MaxCount=1,
     InstanceType='t2.micro'
 )

print(instances[0].id)

# Delete a EC2 Instance

instance_id='i-0703888839d932170'
instance=ec2.Instance(instance_id)
responce=instance.terminate()
print(responce)

```
