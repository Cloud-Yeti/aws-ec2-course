## Lab 8 : Cloudwatch unified agent. Custom Metrics and Instance Logs on Amazon Linux AMI
https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/QuickStartEC2Instance.html

1)  First of all Add required IAM roles to the EC2 instance 
  - In the list of policies while creating IAM Role for EC2 Instance, select the check box next to CloudWatchAgentServerPolicy. Use the search box to find the policy, if necessary.
  
2) Launch an EC2 instance like in Lab 1 

3) SSH into the instance 

4) Find the agent download link here: 
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/install-CloudWatch-Agent-on-first-instance.html

5) Download the Cloudwatch Unified Agent. Find the right agent link for your OS by visiiting the above link
```console
wget https://s3.amazonaws.com/amazoncloudwatch-agent/amazon_linux/amd64/latest/amazon-cloudwatch-agent.rpm
```


6) Install the Cloudwatch Agent 
```console
sudo rpm -U ./amazon-cloudwatch-agent.rpm
```

7) Configure the Cloudwatch agent with the help of a setup wizard: 

```
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-config-wizard
```

Choose all the default option except don't install statd and collectd. And for the log file to monitor select /var/log/httpd/access_log


8) Start the agent .


```
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl -a fetch-config -m ec2 -c file:/opt/aws/amazon-cloudwatch-agent/bin/config.json -s
```

9) You should be set! We'll explore the collected Logs and Metrics individually in the next 
