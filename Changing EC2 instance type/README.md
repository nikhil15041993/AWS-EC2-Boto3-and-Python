## Modifying EC2 instance attributes using Boto3
To change EC2 instance attributes, you can use the modify_attribute() method of the EC2 resource.

Note: You can specify only one attribute at a time. In addition, some attribute changes require the instance to be in a stopped state at the time of the change.
