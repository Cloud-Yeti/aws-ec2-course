## Lab02 create a windows ec2 and login with rdp

- Login to AWS console 
- From the top Navigation Bar/menu Click Services 
- Select ec2 service
- Click on Launch Instance
- Choose Windows 2016 AMI 
- Choose EC2 Instance Type of t2.micro
- Configure Instance
  - There are many parameters  we can configure  but for this lab, we will leave them default. 
- Click "Next:Add Storage" leave it default
- Click "Next: Add Tags" and Tag Instance
- Configure Security Group
- Click Review and Launch Instance
- Create a Key Pair, download it  , check the I Acknowledge box and Launch Instance.

Your instance will now launch. 

- Click Connect
- Decrypt Password by supplying the key pair
- Use Microsoft Remote desktop to login.

