## Lab2-create-a-spot-instance.MD
-Spot Instances can be requested using the AWS Management Console or Amazon EC2 APIs. To start with the AWS Management Console simply:

- Log in to the AWS Management Console, then click the “Amazon EC2” tab.
- Click on “Spot Requests” in the navigation pane on the left.
- Click on “Pricing History” to open a view of historical pricing selectable by instance type. This will help you choose a maximum price for your request. Pricing shown is specific to the Availability Zone selected. If no Availability Zone is selected, you will see the prices for each Availability Zone in the Region.
- Click on “Request Spot Instances” and proceed through the Launch Instance Wizard process, choosing an AMI and instance type. Enter the number of Spot Instances you would like to request, your maximum price and whether the request is persistent or not. After choosing your key pair and security group(s), you are ready to submit your Spot Instance request.

Source:
- https://aws.amazon.com/ec2/spot/spot-getting-started/
