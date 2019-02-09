## Lab 09 : Cloudwatch Metrics

In the last lab we configured the cloudwatch Unified agent. Now let's look at the metrics collected by the agent. 

Remember: RAM/Memory metrics are not collected by Cloudwatch. Cloudwatch agent enables us to collect those metrics not collected by default.\


In the config wizard we selected to collect Metrics like Ram etc.\


## Steps
1. Navigate to Cloudwatch Management Console 
![image](https://user-images.githubusercontent.com/22568316/51443494-8e175f00-1cb7-11e9-94a5-d738cdaa5cad.png)

2. On the left navigation pane select Metrics and you should see a window like this:
![image](https://user-images.githubusercontent.com/22568316/51443506-adae8780-1cb7-11e9-89b3-aecb59a641fc.png)

3. Click on the CWAgent. This is the metrics sent by the Unified cloudwatch agent 
![image](https://user-images.githubusercontent.com/22568316/51443506-adae8780-1cb7-11e9-89b3-aecb59a641fc.png)

4). Click on the ImageId, InstanceId, InstanceType Box
![image](https://user-images.githubusercontent.com/22568316/51443521-ea7a7e80-1cb7-11e9-86df-0ce2b046c8e8.png)


5) Select/Check  the Mem Used metric and you should see something like this 
![image](https://user-images.githubusercontent.com/22568316/51443528-0c740100-1cb8-11e9-9b11-b80a9df0c049.png)


6) Congratulations! you just collected and graphed EC2 Custom metrics using the Cloudwatch Unified Agent

7) Now let's add another custom metric by changing the config file:







