# Compute 

<details>
<summary>Do T2 instances persist their credit balance through a stop/start?</summary>
No
<br></details>

<details>
<summary>KVM stands for _____, and is used for Linux Hypervisor Virtualization.</summary>
Kernel Virtual Machine&nbsp;
<br></details>

<details>
<summary>Required before creating an instance group</summary>
Instance template
<br></details>

<details>
<summary>EC2 available virtualization types</summary>
<b>PV</b>Para-Virtual
<b>
</b><b>HVM</b>Hardware Virtual Machine
<br></details>

<details>
<summary>Can you add a role to an EC2 instance after it has been created and started?</summary>
No
<br></details>

<details>
<summary>Are reserved instances available for multi-AZ deployments?</summary>
Yes
<br></details>

<details>
<summary>Is it possible to transfer a reserved instance from one Availability Zone to another?</summary>
Yes
<br></details>

<details>
<summary>Is Docker supported on Elastic Beanstalk?</summary>
Yes
<br></details>

<details>
<summary>Can you switch AZ's on an existing reserved instance?</summary>
Yes
<br></details>

<details>
<summary>A placement group is ideal for _____&nbsp; that require high network throughput and low latency across a single availability zone.</summary>
EC2 instances
<br></details>

<details>
<summary>A role has been assigned to an existing EC2 instance. Can you change the role's permissions?</summary>
Yes, and the changes will take effect immediately.
<br></details>

<details>
<summary>You have an EC2 instance which needs to find out its private and public IP's. To do this you need to...</summary>
Fetch its meta-data from http://169.254.169.254/latest/meta-data/
<br></details>

<details>
<summary>An application on EC2 must call AWS API's. How should you securely <b>pass credentials</b> to it?</summary>
Use IAM roles for the instances.
<br></details>

<details>
<summary>An application will need to keep network traffic the lowest latency possible while leveraging very high CPU performance on AWS. What are some of the things you could suggest for deployment?</summary>
Use CPU optimized EC2 instances deployed into placement groups
<br></details>

<details>
<summary>When creating <u>resource level permissions,</u>&nbsp;the 4 actions of an EC2 instance that you can control, are...</summary>
START / RESTARTSTOP / TERMINATE
<br></details>

<details>
<summary>Where do you configure your instance's&nbsp;<b>Placement Groups</b>?</summary>
In the Auto Scaling Group
<br></details>

<details>
<summary>It's a best practice to keep dynamic data closer to the _____ and static data closer to the _____</summary>
compute&nbsp;
&nbsp;end-user
<br></details>

<details>
<summary>What 4 attributes of an instance must your RI match to cover it?</summary>
AZ, instance type, platform, Tenancy
<br></details>

<details>
<summary>Instance type modifications are supported for Linux/UNIX platform reservations if...&nbsp;</summary>
The platform isn't licensed (like RedHat)
<br></details>

<details>
<summary>An application runs 24/7 on EC2, and the load is predictable and constant throughout the year. The most cost-efficient EC2 purchase model in this case is...</summary>
EC2 Reserved
<br></details>

<details>
<summary>A reserved instance can save you money over on-demand instances. If you shut down the reserved instance, will the hourly charge incur for the shutdown hours?</summary>
No
<br></details>

<details>
<summary>Does the data on the instance based storage remains intact when you reboot the EC2 instance?</summary>
Yes
<br></details>

<details>
<summary>How many VMs should usually allocate to Cloud Vision?</summary>
None; Cloud Vision is a serverless service.
<br></details>

<details>
<summary>You can use AWS _____ to analyze images and extract text seen in the image.</summary>
Cloud Vision
<br></details>

<details>
<summary>If the AMI changes, but it's the same instance type, is the Reserved instance still valid?</summary>
Yes
<br></details>

<details>
<summary>Can I move a reserved instance from one region to another?</summary>
No
<br></details>

<details>
<summary>You are designing a new web application which will need to access data stored in DynamoDB. You need to do this as securely as possible, without storing any credentials on a long term basis. How would you achieve this?</summary>
AWS IdentityIAM roles for the API-calling EC2 Instances
<br></details>

<details>
<summary>Can an AMI be copied to another region?</summary>
Yes - It will get a new ami ID though
<br></details>

<details>
<summary>Can you SSH into ElasticBeanstalk instances?</summary>
Yes
<br></details>

<details>
<summary>With ElasticBeanstalk can you deploy from a zip file with code?</summary>
Yes
<br></details>

<details>
<summary>Can you move an RI from one region to another?</summary>
No
<br></details>

<details>
<summary>The <b>/dev/sda1/</b>&nbsp;name in EC2 is reserved for the _____ device</summary>
root
<br></details>

<details>
<summary>Can you create an instance store-backed AMI?</summary>
Yes
<br></details>

<details>
<summary>Can Auto Scaling start/release EC2 instances when CPU utilization is above/below threshold?</summary>
Yes
<br></details>

<details>
<summary>Can Auto Scaling increase instance sizes when utilization is above threshold?</summary>
No
<br></details>

<details>
<summary>Can auto scaling reboot an instance if its health check has failed?</summary>
No
<br></details>

<details>
<summary>In an EC2 instance, can you use instance based storage for your root volume?</summary>
Yes
<br></details>

<details>
<summary>Can you restrict who has access to specific EC2 instances via SSH keys and passwords?</summary>
Yes
<br></details>

<details>
<summary>A Reserved Instance is associated with a specific instance type for the duration of its term; however, you can change from one instance size (e.g., c3.large) to another (e.g., c3.xlarge) in the same type, if...</summary>
If it is a Linux/UNIX Reserved Instance.&nbsp;
<br></details>

<details>
<summary>Specifying the mapping <b>/dev/sdc=none</b> prevents /dev/sdc from _____ when launching an EC2 instance.</summary>
Attaching to the instance.
<br></details>

<details>
<summary>Are reserved Instances available for Multi-AZ Deployments?</summary>
Yes
<br></details>

<details>
<summary>Can you share your AMI with other AWS account owners?</summary>
Yes
<br></details>

<details>
<summary>For Instance stored-backed AMIs, where is the root volume stored?</summary>
S3
<br></details>

<details>
<summary>With ElasticBeanstalk can you deploy from a repo with code?</summary>
Yes
<br></details>

<details>
<summary>Is an EC2 instance's storage automatically saved in S3?</summary>
No
<br></details>

<details>
<summary>Can you limit who has access to a specific EC2 instance via IAM?</summary>
No
<br></details>

<details>
<summary>You have a high performance compute application and you need to minimize network latency between EC2 instances as much as possible. What can you do to achieve this?</summary>
Create a placement group within an Availability Zone and place the EC2 instances within that placement group.
<br></details>

<details>
<summary>Are EC2 instance store volumes wiped on a REBOOT?</summary>
No
<br></details>

<details>
<summary>Do all instances in a placement group have to be of the same instance type?</summary>
Yes
<br></details>

<details>
<summary>A _____ allows you to&nbsp;manage and&nbsp;<i>automatically</i>&nbsp;bid on multiple Spot instances that provide the lowest price per unit.</summary>
Spot fleet
<br></details>

<details>
<summary>A stopped instance will be started as part of the cluster placement group it was in when it stopped. What happens if capacity is not available for it to start within its cluster placement group?</summary>
The start will fail
<br></details>

<details>
<summary>When transferring data from an EC2 instance in one AZ to an EC2 instance in another AZ, you would be charged for data input and output, specifically _____ the first instance, and _____ the second.</summary>
out
in
<br></details>

<details>
<summary>Will I be charged if my Spot EC2 instance is terminated by Amazon before the hour is up?</summary>
No
<br></details>

<details>
<summary>_____ volumes are virtual devices whose underlying hardware is physically attached to the host EC2 instance</summary>
Instance store
<br></details>

<details>
<summary>You can have ____ EC2 instances per region</summary>
20
<br></details>

<details>
<summary>In auto scaling you can scale by an integer or by ____</summary>
A percentage of your max ASG size
<br></details>

<details>
<summary>If you delete an Autoscaling group will the instances spun up by it be deleted?</summary>
Yes
<br></details>

<details>
<summary>If an instance in a cluster placement group is stopped then started again, will it maintain its presence in the cluster placement group?</summary>
Yes.&nbsp;
<br></details>

<details>
<summary>You want to add a second EC2 instance for your application that requires a high bandwidth connect with the existing EC2. You should launch your EC2's in a _____ in this case.</summary>
Placement Group
<br></details>

<details>
<summary>An EC2 instance on a public subnet needs an _____ or _____ to be Internet accessible.</summary>
ELB or Elastic IP
<br></details>

<details>
<summary>If an EC2 instance is unhealthy, what will its ELB do?</summary>
Stop sending traffic to that instance
<br></details>

<details>
<summary>Newly created EC2 instances can have a Public IP automatically assigned to them by enabling _____</summary>
"Auto-assign Public IP"
<br></details>

<details>
<summary>A Spot EC2 Instance request is made by specifying the instance type, the desired number of instances and Availability Zone, and finally the maximum price to pay per _____</summary>
instance hour.
<br></details>

<details>
<summary>Can EC2 placement group&nbsp;<span style="font-family: Arial;">be deployed across multiple Availability Zones?</span></summary>
No
<br></details>

<details>
<summary>Does the public DNS of an EC2 instance remain intact when you shut it down and start it again?</summary>
No
<br></details>

<details>
<summary>Micro instances have a fraction of the compute resources that Standard Small instances do.&nbsp;However, they can be set to temporarily _____ to up to 2 ECUs.</summary>
burst
<br></details>

<details>
<summary>Can EC2 instances have credentials stored on them so that the instances can access other resources (such as S3 buckets)?</summary>
No - You should be assigning <b>roles</b>.
<br></details>

<details>
<summary>Can you schedule reserved instances for certain days/times?</summary>
Yes
<br></details>

<details>
<summary>Can you configure Availability Zones in the Auto Scaling Group?</summary>
Yes
<br></details>

<details>
<summary>What type of memory does EC2 use?</summary>
ECC
<br></details>

<details>
<summary>Any emergent change to the EC2 Spot instance price won't reflect on the billing until _____</summary>
Until the next instance-hour begins.
<br></details>

<details>
<summary>1 CPU credit provides one _____ of a full CPU core on T2 burstable instances.</summary>
minute
<br></details>

<details>
<summary>You can attach up to _____ Elastic Network Interfaces to an instance.</summary>
2
<br></details>

<details>
<summary>Do you need an ELB for Auto Scaling?</summary>
Yes
<br></details>

<details>
<summary>Does auto-scaling your EC2 instances across availability zones such that a number of instances must always run inside each, help at all to make your application highly available?</summary>
Yes
<br></details>

<details>
<summary>An EC2 is connected to an Elastic Network Interface in one subnet. If you try to attach another subnet's ENI to the instance, the instance will follow the rules of _____</summary>
both subnets
<br></details>

<details>
<summary>An EC2 instance is launched in a private subnet. Using an Internet Gateway, are you able to route the instance's traffic to a NAT in a public subnet?</summary>
Yes
<br></details>

<details>
<summary>Does Elastic Beanstalk automatically handle the deployment, capacity provisioning, load balancing, auto-scaling and application health monitoring based on the code you upload to it?</summary>
Yes
<br></details>

<details>
<summary>Can you attach multiple Elastic IPs to a single EC2 instance?</summary>
No
<br></details>

<details>
<summary>If using an ELB, Auto Scaling health checks can be configured to use the _____ checks of the ELB.</summary>
status checks
<br></details>

<details>
<summary>If your maximum spot instance price bid exceeds the current spot instance price, instances will be started and run until either they are terminated, or ______</summary>
the spot instance price increases above your maximum price bid.
<br></details>

<details>
<summary>To make an application highly available, does it help to spread its EC2 instances across availability zones and regions, with an ELB balacing the load?</summary>
Yes
<br></details>

<details>
<summary>Individual instances are provisioned within _____</summary>
Availability Zones
<br></details>

<details>
<summary>Can you configure auto scaling groups have auto-scaling schedules?</summary>
Yes - in the ASG scheduling tab.
<br></details>

<details>
<summary>What happens to my Amazon EC2 instances if I delete my Auto Scaling Group?</summary>
They're terminated
<br></details>

<details>
<summary>A large data analysis requires high computing power and many instances to be launched simultaneously and then to be retired after the analysis. If the instance is retired during the analysis, the program automatically shifts the analysis to the other instance. Which is the most cost-efficient option for launching the EC2 in this case?</summary>
Spot
<br></details>

<details>
<summary>Will I be charged for the hour if I terminate a spot instance myself?</summary>
Yes
<br></details>

<details>
<summary>Do you need CloudWatch for Auto Scaling?</summary>
Yes - auto scaling activates based on metrics.
<br></details>

<details>
<summary>Do you get root access to EC2 and Elastic MapReduce?</summary>
Yes
<br></details>

<details>
<summary>In EC2 if your limit for instances is 20, you can have how many total?</summary>
40 if 20 are stopped
<br></details>

