# Networking 

<details>
<summary>Can an instance on a public subnet (e.g. has an IGW) browse the web (i.e. outbound traffic) if it doesn't have a public IP?</summary>
No. (Tested this)
<br></details>

<details>
<summary><b>CloudFront&nbsp;</b>Are the choice of edge location chosen for a user's request is dependent on a DNS check?</summary>
Yes
<br></details>

<details>
<summary>How does CloudFront determine which edge location to use for a user?</summary>
Latency Based Routing (DNS)
<br></details>

<details>
<summary>Are CloudFront template names unique within your entire AWS account?</summary>
Yes
<br></details>

<details>
<summary>In Route 53, why might a CloudFront distribution not be showing up as an available endpoint?</summary>
Your CF distribution has no "Alternate Domain Name"
<br></details>

<details>
<summary>Can DNS issue cause perf issues?</summary>
Yes
<br></details>

<details>
<summary>VPCCan have ____ IGWs</summary>
1
<br></details>

<details>
<summary><b>ELB</b>What may cause it to stop sending traffic to instances in multiple AZ's?</summary>
AZ's not added to the ELB. &nbsp;

Cross-AZ load balancing disabled.
<br></details>

<details>
<summary>How is inbound traffic in AWS ensured it's coming from the real source?</summary>
Packet Filtering
<br></details>

<details>
<summary>Do placement groups require instances to have Ehanced Networking enabled?</summary>
Yes
<br></details>

<details>
<summary><b>ELB Public</b>Needs at least ____ subnets added to work</summary>
2
<br></details>

<details>
<summary>ELB&nbsp;Connection draining is...</summary>
ELB waits for connections to the EC2 instance to close before removing the instance
<br></details>

<details>
<summary>In a default AWS VPC, does any subnet automatically has a route to all other subnets regardless whether private/public?</summary>
Yes
<br></details>

<details>
<summary>To browse the web, a machine on a private subnet with a public IP needs:</summary>
An Internet Gateway and NAT Gateway
<br></details>

<details>
<summary>A NAT instance can forward traffic from other instances if...</summary>
Source/Destination checks are disabled
<br></details>

<details>
<summary>VPC&nbsp;Where to define your on-premise firewall/router public IP?</summary>
Customer Gateway
<br></details>

<details>
<summary><b>Direct Connect</b>Has VPC Peering</summary>
No
It connects on-prem to a VPC
<br></details>

<details>
<summary>ELBHow can you point the root of your domain to an ELB?</summary>
Route53 alias
<br></details>

<details>
<summary>Direct Connect&nbsp;Requires hardware in your data center?</summary>
No, just a participating backbone provider&nbsp;(e.g. Verizon)
<br></details>

<details>
<summary><b>Direct Connect</b>&nbsp;Requires a _________ per VPC you're connecting to.</summary>
Private Virtual Interface
<br></details>

<details>
<summary><b>Route53&nbsp;</b>Weighted Routing Policy</summary>
Route traffic by percentages
<br></details>

<details>
<summary>What is VPN CloudHub?</summary>
A hub for on-prem datacenters
<br></details>

<details>
<summary><b>Direct Connect</b>&nbsp;Requires ____ protocol routing</summary>
Border Gateway (BGP)
<br></details>

<details>
<summary><b>Route tables</b>How to route connections to the Internet from your subnet?</summary>
<b>Destination: 0.0.0.0/0</b><b>
</b><b>Target: IGW</b>
<br></details>

<details>
<summary>Route53 Latency Based RoutingUse cases</summary>
Choosing AWS Regions with the best latency

Multi-regional apps
Multi-regional failover
<br></details>

<details>
<summary>Can a placement group span multiple VPCs?</summary>
Yes
<br></details>

<details>
<summary>A Virtual Private Gateway can be referenced by ____ VPN connections</summary>
10
<br></details>

<details>
<summary>ELBAre just EC2 instances auto-scaling based on traffic, with load balancing software installed?</summary>
Yes
<br></details>

<details>
<summary><b>Subnets</b>Are configured in...</summary>
The Auto-Scaling Group
<br></details>

<details>
<summary>ELB&nbsp;caps the number of connections sent to your internal web servers?</summary>
No
<br></details>

<details>
<summary>If you want an EC2 instance to have a public IP address, you can attach _____</summary>
An Elastic IP
<br></details>

<details>
<summary>To establish a VPN connection between an on-premises data center and an Amazon VPC virtual private gateway, you might assigned a public, static IP address to an Amazon _____ gateway.</summary>
Customer
<br></details>

<details>
<summary>Can new subnets communicate with each other across Availability Zones in a custom AWS VPC?</summary>
By default yes
<br></details>

<details>
<summary>Amazon VPC is the networking layer for ____</summary>
EC2
<br></details>

<details>
<summary>Enable Internet access to an instance</summary>
Attach IGW to VPC
Add a route between subnet and IGW
Check ACLs / security groups rules if still no good
<br></details>

<details>
<summary>Direct Connect&nbsp;You can hit <i>public endpoints</i> over a <i>private</i> connection and AWS's backbone only without hitting the internet using</summary>
Public Virtual Interfaces
<br></details>

<details>
<summary>Direct ConnectEnables connectivity to the closest geographic region and others?</summary>
Yes
<br></details>

<details>
<summary>For Route53 to direct your "www." sub-domain to an ELB in front your web servers, you should set a _____ record.</summary>
CNAME
<br></details>

<details>
<summary>A VPC subnet is considered "public" if it has at least one route in its associate _____ that uses an Internet Gateway.</summary>
routing table
<br></details>

<details>
<summary>A _____ acts as a firewall that controls the traffic allowed to reach one or more instances.&nbsp;</summary>
Security Group
<br></details>

<details>
<summary>Which Amazon service can I use to define a virtual network that resembles a data center?</summary>
Amazon VPC
<br></details>

<details>
<summary><b>Route tables</b>purpose</summary>
Sets rulesDetermining where traffic from subnets / gateways is directed
<br></details>

<details>
<summary>AWS&nbsp;Provide port scanning protection?</summary>
Yes
<br></details>

<details>
<summary>An _____ can be attached to a VPC to enable traffic between resources and the Internet</summary>
Internet Gateway
<br></details>

<details>
<summary>Can you launch AWS resources into a specific subnet?</summary>
Yes
<br></details>

<details>
<summary><b>VPC</b>How to enable IPV4 outbound-only communication?</summary>
NAT Gateway
<br></details>

<details>
<summary>In a VPC
What is the Route 53 DNS IP?</summary>
VPC CIDR range + 2 &nbsp;
Ex.:<b>VPC CIDR&nbsp;</b>172.31.0.0/16&nbsp;
<b>DNS Server</b>172.31.0.2
<br></details>

<details>
<summary>VPCA security group can have ____ rules</summary>
50
<br></details>

<details>
<summary>Can you peer VPC's across regions?</summary>
No
<br></details>

<details>
<summary>An AWS region can have ____ VPCs</summary>
5
<br></details>

<details>
<summary>VPC CustomAn instance launched into a custom VPC receives a public ip by default</summary>
No
<br></details>

<details>
<summary>AWS Route53 can have ____ max domain names</summary>
50 (upgradable)
<br></details>

<details>
<summary>Can a placement group span multiple regions?</summary>
No
<br></details>

<details>
<summary>A VPC can have ____ subnets</summary>
20
<br></details>

<details>
<summary>A VPC can have ____ VPN connections.</summary>
10
<br></details>

<details>
<summary>Direct Connect&nbsp;Can connect VPCs in different regions?</summary>
Yes
<br></details>

<details>
<summary>Can a subnet span multiple AWS availability zones?</summary>
No
<br></details>

<details>
<summary>An AWS Region can have ____ VPCs</summary>
5
<br></details>

<details>
<summary>Does VPC support ipv6?</summary>
No
<br></details>

<details>
<summary>An AWS VPC can have ____ Virtual Private Gateways</summary>
1
<br></details>

<details>
<summary>VPC
A region can have ____ security groups</summary>
500
<br></details>

<details>
<summary>Route53&nbsp;Supports Apex records (naked domain names)?</summary>
Yes
<br></details>

<details>
<summary>A VPC can have ____ security groups</summary>
500
<br></details>

<details>
<summary>Does an instance launched into the default VPC receive a public IP?</summary>
Yes
<br></details>

<details>
<summary>AWS AZ means</summary>
Availability Zone
<br></details>

<details>
<summary>ELB&nbsp;Supports ipv6?</summary>
Yes
<br></details>

<details>
<summary>What is a public subnet in an AWS VPC?</summary>
One with atleast one IGW route in its table
<br></details>

<details>
<summary><b>VPC Default&nbsp;</b>Does it have a default IGW attached to all 4 default subnets?</summary>
Yes
<br></details>

<details>
<summary>Where are Instance size, AMIs, security groups configured?</summary>
Launch Configuration
<br></details>

<details>
<summary>You have an EC2 security group with several EC2 instances running inside it. You change the security group rules to allow inbound traffic on port 443 and you then launch several new instances in the same security group. How and when do the new rules apply?</summary>
Straight away to all instances within the security group.
<br></details>

<details>
<summary>If you are unable to access your EC2 linux instance via SSH, it could be because the port 22 is closed on the _____ for incoming traffic.</summary>
Security Group
<br></details>

<details>
<summary>Can you restrict who has access to specific EC2 instances via security groups?</summary>
Yes
<br></details>

<details>
<summary>An EC2 security group has several running EC2 instances. You change the security group rules to allow inbound traffic on a new port and protocol, and launch several new instance in the same security group. How and when do the new rules apply?</summary>
Immediately to all present and future instances in the security group.
<br></details>

<details>
<summary>Can an S3 Bucket be a CloudFront origin?</summary>
Yes
<br></details>

<details>
<summary>Can a CloudFront signed url be set to expire after a configurable timeout?</summary>
Yes
<br></details>

<details>
<summary>You need to deploy EC2 instances in to multiple availability zones. What is the minimum number of VPC subnets required?</summary>
One subnet for each AZ
<br></details>

<details>
<summary>A wordpress site is running on an <b>EC2</b> instance with <b>Route53 </b>and <b>ELBs</b>. When you browse the URL, nothing happens. What are some potential causes?</summary>
EC2 instance's security group ports 80/443 are closed
ELB health checks a webpage that does not exist, refusing service.
Missing ALIAS for your A record to point to the ELB
<br></details>

<details>
<summary>A custom VPC has a private subnet with one EC2 instance, and a public subnet with 3 EC2 instances, each with an Elastic IP attached. To give Internet access to the private subnet's instance, you can deploy _____ and then update the main route table to send traffic to the private subnet via it.</summary>
NAT
<br></details>

<details>
<summary>Can peering connections be created across regions?</summary>
No
<br></details>

<details>
<summary>A VPC's rules are as follows: ALLOW port 80, DENY port 80. What happens?</summary>
Port 80 will be allowed. A DENY will have no affect if something is specifically allowed before it.
<br></details>

<details>
<summary>Does Cloudfront allow you to specify an origin based on the kind of device accessing it.</summary>
Yes
<br></details>

<details>
<summary>In CloudFront&nbsp;can you upload to an edge location and have it sync back to the origin?</summary>
Yes - by allowing PUT/POST in "Allowed HTTP Methods"
<br></details>

<details>
<summary>The SR-IOV driver required for Enhanced Networking stands for _____.&nbsp;&nbsp;This driver is in the Amazon HVM Linux AMI's by default. For AMI's that don't have it you can install the driver yourself.</summary>
<b><u>S</u>ingle <u>R</u>oot <u>I/O</u> <u>V</u>irtualization</b>
<br></details>

<details>
<summary>Can Network traffic entering and exiting each subnet can be allowed or denied via network Access Control Lists (ACLs)?</summary>
Yes
<br></details>

<details>
<summary>What could you use to establish a VPN connection between your data center and a VPC virtual private gateway?</summary>
VPC Customer Gateway
<br></details>

<details>
<summary>What's a VPC?</summary>
A virtual network
<br></details>

<details>
<summary>Does an&nbsp;<b>Elastic Network Interface </b>support&nbsp;security groups?</summary>
Yes
<br></details>

<details>
<summary>Can a VPC's subnets communicate with each other across Availability Zones by default?</summary>
Yes - using the main route table
<br></details>

<details>
<summary>Can an ELB be a CloudFront origin?</summary>
Yes
<br></details>

<details>
<summary>_____ URLs can be created to access objects from CloudFront edge locations</summary>
Signed
<br></details>

<details>
<summary>Can a subnet span multiple regions?</summary>
No
<br></details>

<details>
<summary>Can Glacier be used as a CloudFront origin server?</summary>
No
<br></details>

<details>
<summary>You are designing an image sharing website that will distribute images across the world. You need maximise performance so that your end users can download frequently accessed images as fast as possible. What AWS technology should you implement?</summary>
CloudFront
<br></details>

<details>
<summary>When are CloudFront edge location caches updated?</summary>
When something is requested
<br></details>

<details>
<summary>How do you point your website's apex record to the public DNS of an ELB?</summary>
ALIAS
<br></details>

<details>
<summary>You have created 4 weighted resource record sets with weights 1, 2, 3 and 4. The 3rd record set is selected by Route53 _____% of the time.</summary>
30%
<br></details>

<details>
<summary>Can a personal webserver be used as an origin server in CloudFront?</summary>
Yes
<br></details>

<details>
<summary>When content is missing at a CloudFront edge location and a request is made to it, CloudFront delivers content from _____ and caches it</summary>
the origin
<br></details>

<details>
<summary>The best way to route a website’s traffic to an ELB is to create a Route53 _____ record for the website, pointing it to the ELB's DNS name.</summary>
CNAME
<br></details>

<details>
<summary>A subnet is a range of _____ in a VPC</summary>
IP addresses
<br></details>

<details>
<summary>CloudFront optimises video livestreams by cache media at the edges and combining them in the _____</summary>
client
<br></details>

<details>
<summary>Network ACLs restrict traffic to a _____</summary>
subnet
<br></details>

<details>
<summary>Does a VPC always exist across multiple AZ's in a region?</summary>
Yes
<br></details>

<details>
<summary>Can a CloudFront signed url be set to expire after a certain number of uses?</summary>
Yes
<br></details>

<details>
<summary>Direct access to S3 URLs can be _____ therefore allowing access only through CloudFront URLs</summary>
removed&nbsp;
<br></details>

<details>
<summary>Can an S3 bucket be used as a CloudFront origin server?</summary>
Yes
<br></details>

<details>
<summary>A user requests a file in CloudFront, which routes them to the nearest _____ via DNS.</summary>
edge location
<br></details>

<details>
<summary>You can override S3 bucket permissions in CloudFront by using an _____ identity.</summary>
origin access
<br></details>

<details>
<summary>In CloudFront you can create different behaviors like cache timeout using _____</summary>
Patterns
<br></details>

<details>
<summary><i>Auto Scaling</i> health checks use the ____ status checks by default.</summary>
instance
<br></details>

<details>
<summary>A limitation of using S3 for a failover page is that the <b>bucket name </b>needs to match the <b>domain name</b>. But with _____ you can configure&nbsp;multiple alternate domain names&nbsp;on the distribution.</summary>
CloudFront
<br></details>

<details>
<summary>Can it be cheaper and faster to deliver content via CloudFront than directly from S3?</summary>
Yes
<br></details>

<details>
<summary>Is there an additional charge for enhanced networking?</summary>
No
<br></details>

<details>
<summary>Using CloudFront, to serve content that is stored in S3, but not publically accessible from S3 directly, you could create an _____ and grant it access to your S3 bucket objects.</summary>
Origin Access Identity (OAI)
<br></details>

<details>
<summary>A VPC network must support two applications: one internet-facing and one only accessible internally over VPN. Both applications must leverage at least three AZs for high availability. How many subnets must you create within your VPC to accommodate these requirement at minimum?</summary>
6
<br></details>

<details>
<summary>To ensure failover capabilities, consider using a secondary _____ IP for incoming traffic on a network interface.</summary>
private
<br></details>

<details>
<summary>Peforming NAT for instances assigned a Public IP and providing a target for route tables are some of the purposes of an <b>_____</b></summary>
Internet Gateway
<br></details>

<details>
<summary>Link your infrastructure to AWS directly via fiber, you could use _____</summary>
Direct Connect
<br></details>

<details>
<summary><div style="font-family: Arial;"><span style="font-family: &quot;Liberation Sans&quot;;">In a default VPC, each EC2 instance is assigned a _____ IP and a _____ IP.</span></summary>
Private IP and Public IP
<br></details>

<details>
<summary>Can you put a CNAME on the apex of a domain?</summary>
No
<br></details>

<details>
<summary><font face="Arial">To&nbsp;enable outbound-only IPV6 communication, you could use an Egress _____</font></summary>
Egress Internet Gateway
<br></details>

<details>
<summary>Can Security Groups be nested?</summary>
No
<br></details>

<details>
<summary>Can Security Groups work outside of a VPC?</summary>
Yes
<br></details>

<details>
<summary>In Amazon VPC, does an instance retain its private IP address when the instance is stopped?</summary>
Yes
<br></details>

<details>
<summary>Default subnets are assigned a /_____ netblocks</summary>
/20
<br></details>

<details>
<summary>Can a subnet span multiple availability zones?</summary>
No
<br></details>

<details>
<summary>When adding a rule to an RDS security group, do you need to specify the protocol and port?</summary>
Yes
<br></details>

<details>
<summary>In a newly created security group, all outbound traffic is _____ by default.</summary>
allowed
<br></details>

<details>
<summary>A public subnet has EC2 instances running inside an autoscaling group, all of which are in the same security group. An application running on these instances requires a specific port to be opened in order to be globally accessible to devices on the Internet. What could you do to allow these instances to communicate over this port immediately?</summary>
Open the required port on the security group.
<br></details>

<details>
<summary>In an EC2 instance, how can you find your own IP address?</summary>
curl http://169.254.169.254/latest/meta-data/
<br></details>

<details>
<summary>Security Groups restrict access to _____</summary>
EC2
<br></details>

<details>
<summary>For an EC2 instance to become accessible from the Internet, you could attach _____</summary>
an Elastic IP
<br></details>

<details>
<summary>Network ACLs are _____ and any return ports must be specifically allowed.</summary>
stateless
<br></details>

<details>
<summary>In a newly created security group, all inbound traffic is _____ by default.</summary>
forbidden
<br></details>

<details>
<summary>You have an EC2 instance with Internet access, running inside a public subnet. You launch a second instance in the subnet using the same AMI (Amazon Machine Image) and security group configuration, but this instance cannot be accessed fro the Internet. To enable Internet access, you should _____</summary>
Assign an elastic IP address to the second instance.
<br></details>

<details>
<summary>Is transitive VPC peering possible?</summary>
No. Any two pairs need their own peering connections.
<br></details>

<details>
<summary>Is the data transferred over Direct Connect billed at a lower rate?</summary>
Yes
<br></details>

<details>
<summary>A Security Group default settings are to _____ inbound traffic and _____ outbound traffic.</summary>
DENY inbound traffic
ALLOW outbound traffic
<br></details>

<details>
<summary>Is it mandatory to&nbsp;assign at least one&nbsp;Security Group&nbsp;to your server?</summary>
Yes
<br></details>

<details>
<summary>When an EC2 instance is stopped, does it retain its private IP address indefinitely?</summary>
Yes
<br></details>

<details>
<summary>When an S3 bucket is marked private, you can create an _____ to access the objects via CloudFront</summary>
Origin Access Identity
<br></details>

<details>
<summary>Security groups are _____, meaning they track inbound sessions to allow outgoing over any port.</summary>
stateful
<br></details>

<details>
<summary>Is an Internet Gateway horizontally scalable?</summary>
Yes
<br></details>

