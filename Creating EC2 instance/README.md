## Creating EC2 instance

To create one or more EC2 instances, you need to use the create_instances() method

```

MinCount – minimum number of EC2 instances to launch
MaxCount – maximum number of EC2 instances to launch
ImageId – the Amazon Machine Image which is used to launch your EC2 instance (Working with Snapshots and AMIs using Boto3 in Python)
InstanceType – Instance Type specifies how much CPU and RAM resources your EC2 instance should have
KeyName – SSH key name, which you’re going to use to get remote access to the EC2

```

Thecreate_instances() method returns a list of launched instances. You can use the fol-loop to walk through the instances and wait till every instance is up and running if you need to (thewait_until_running() method).
