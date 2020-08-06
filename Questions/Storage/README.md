# Storage 

<details>
<summary>You provision an EBS volume, but it appears to run at a slow rate of IOPS through no apparent fault of your own. Why might that be?</summary>
AWS always wipes the physical disk from its last usage, so you might experience slower IOPS until it has finished.
<br></details>

<details>
<summary>With Auto scaling groups, where do you configure instance tags?</summary>
The ASG!
<br></details>

<details>
<summary>_____ let you categorize your EC2 resources in different ways, for example, by purpose, owner, or environment.</summary>
tags&nbsp;
<br></details>

<details>
<summary>To help you manage your Amazon EC2 instances you can assign your own metadata in the form of</summary>
Tags
<br></details>

<details>
<summary>How can objects be organized?</summary>
Names
Prefixes

Metadata

S3 object lifecycle tags
S3 inventory
<br></details>

<details>
<summary>Cost Allocation S3 bucket tags help with...</summary>
Tracking storage costs and other criteria on S3 by organizing your billing report
<br></details>

<details>
<summary><b>bucket policy</b>use cases</summary>
grant permissions to users 
(in an AWS account)
Manage cross-account permissions
<br></details>

<details>
<summary>How many S3 buckets can I have per account by default?</summary>
100
<br></details>

<details>
<summary>How to add tags to many objects with a single request?</summary>
S3 Batch Operations
<br></details>

<details>
<summary>Can a bucket owner allow unauthenticated requests/uploads?</summary>
Yes - as "<b>public bucket</b>" policy or by a <b>WRITE/FULL_CONTROL</b>&nbsp;for <b>All Users ACL</b>
<br></details>

<details>
<summary>bucket subresources</summary>
cors
website
logging
versioning
lifecycle
policy and acl
<br></details>

<details>
<summary>You are designing a site for a new start up which generates cartoon images for people automatically. Customers will log on to the site, upload an image which is stored in S3. The application then passes a job to AWS SQS and a fleet of EC2 instances poll the queue to receive new processing jobs. These EC2 instances will then turn the picture in to a cartoon and will then need to store the processed job somewhere. Users will typically download the image once (immediately), and then never download the image again. What is the most commercially feasible method to store the processed images?</summary>
Store the images on S3 RRS, and create a lifecycle policy to delete the image after 24 hours.
<br></details>

<details>
<summary>You can have ____ tags on an object</summary>
10
<br></details>

<details>
<summary>What are the valid methodologies for encrypting data on S3?</summary>
SSE-CSSE-S3
SSE-KMSS3 Encryption Client (or another client library)
<br></details>

<details>
<summary>A business can tolerate losing some of their S3 objects, as they can be regenerated. However, they must be stored persistently and retrieved immediately. Which storage class could be cheapest for this case?</summary>
RRS
<br></details>

<details>
<summary>With Glacier, you can retrieve up to _____ of your average monthly usage each month.</summary>
5%
<br></details>

<details>
<summary>In S3 Lifecycle,&nbsp;<b>Transition </b>actions define when objects _____,&nbsp;<b>Expiration </b>actions define when objects _____</summary>
Moves to another <b>storage class</b><b>
</b>Are deleted
<br></details>

<details>
<summary>A bucket owner has some permissions over another account's objects. These are...</summary>
Access denial

Archival
Deletion
Restoration
<br></details>

<details>
<summary>In<b> S3 Batch Operations, </b>a logical unit of work made up of Operations is a...&nbsp;</summary>
Job
<br></details>

<details>
<summary>To allow anonymous access to an S3 bucket, you would use...</summary>
bucket policy
<br></details>

<details>
<summary>To restrict access to a bucket based on referrer, you would use...</summary>
bucket policy
<br></details>

<details>
<summary>Capability policies are applied on an IAM _____ or _____</summary>
user or group
<br></details>

<details>
<summary>Largest filesize you can upload in a single PUT operation</summary>
5GB
<br></details>

<details>
<summary>An S3 object's data is encrypted using AWS encryption solutions. Is its metadata also encrypted?</summary>
No! Don't store secrets in there!
<br></details>

<details>
<summary>Each S3 Object is uniquely identified by its containing _____, its _____ and its current _____</summary>
BucketKeyVersion
<br></details>

<details>
<summary>You could make an S3 bucket routable only inside your AWS network via...</summary>
An S3 access point that accepts requests only from your VPC
<br></details>

<details>
<summary>The storage class _____ cheaply stores object data in a one Availability Zone only, and therefore is neither as available nor resilient from data center disasters.</summary>
S3 One Zone-IA
<br></details>

<details>
<summary><b>Storage Class minimum storage durations</b></summary>
IA - 30 days

S3 Glacier - 90 days

S3 Glacier Deep Archive - 180 days
<br></details>

<details>
<summary>In a versioning-enabled bucket, can you change the storage class of an object's specific version?</summary>
No
<br></details>

<details>
<summary>S3 VersioningCan you delete a specific version?</summary>
Yes
<br></details>

<details>
<summary>bucket policy, bucket ACL, object ACL are examples of _____ permissions</summary>
&nbsp;resource-based
<br></details>

<details>
<summary>In a bucket, you can set per object permissions and manage objects not owned by the bucket owner via...</summary>
Object ACL
<br></details>

<details>
<summary>With S3 bucket <b>ACLs</b> you can only grant access to _____ AWS accounts.</summary>
root
<br></details>

<details>
<summary>In S3,&nbsp;<b>PUT / GET requests on new objects</b> have _____ consistency, whereas <b>PUT / DELETE on existing objects</b> has _____ consistency.</summary>
read-write

eventual
<br></details>

<details>
<summary>Can you make an Object's <b>requester</b> pay for its data transfer?</summary>
Yes - via <b>"Requester Pays"</b>
<br></details>

<details>
<summary>S3 Glacier Deep Archive default retrieval time is around _____</summary>
12 hours
<br></details>

<details>
<summary>S3 Glacier Deep Archive "bulk retrieval" reduces Deep Archive _____ costs and returns data in 48 hours.</summary>
retrieval&nbsp;

48
<br></details>

<details>
<summary>Are all S3 storage classes resilient?</summary>
No.&nbsp;<b>S3 One Zone-IA</b>&nbsp;stores data in only one Availability Zone
<br></details>

<details>
<summary>Protect S3 objects from unintended changes via...</summary>
Versioning
<br></details>

<details>
<summary>An&nbsp;<b>S3 Versioned </b>object gets deleted. What happens?</summary>
An artificial delete marker becomes the current version of the object. Retrieving it returns only <b>404 Not Found</b> errors.
<img src="versioning_DELETE_versioningEnabled.png">

All versions still remain in the bucket!!! You can still&nbsp;<b>GET</b>&nbsp;a noncurrent version of an object by specifying its version ID.&nbsp;
<br></details>

<details>
<summary>CORS stands for...</summary>
Cross-Origin Resource Sharing
<br></details>

<details>
<summary>Anonymous modification of public bucket objects' ACLs can be prevented by disabling public write access using _____</summary>
<b>S3 Block Public Access</b>
<br></details>

<details>
<summary>Can S3 Buckets be used for namespace organization?</summary>
Yes
<br></details>

<details>
<summary>Can S3 Buckets be used as units of aggregation for usage reporting?</summary>
Yes
<br></details>

<details>
<summary>Once S3 Glacier completes retrieval, you have _____ hours to access it.</summary>
24
<br></details>

<details>
<summary>How can you manage cost allocation in S3?</summary>
Bucket tags
<br></details>

<details>
<summary>Can enabling S3 versioning increase costs?</summary>
Yes - you might be storing thousands of versions of an object
<br></details>

<details>
<summary>To manage a browser's cross-origin requests to S3 hosted websites, you can use...</summary>
CORS (Cross-Origin Resource Sharing)
<br></details>

<details>
<summary>In S3, you could set up log expiration by using...</summary>
Lifecycles
<br></details>

<details>
<summary>An S3 Glacier retrieval usually completes in around _____ hours.</summary>
5
<br></details>

<details>
<summary>S3 url syntax consists of...
<b>_____</b>.s3.<b>_____</b>.amazonaws.com/<b>_____</b></summary>
<b>BUCKETNAME</b>.s3.<b>REGION</b>.amazonaws.com/<b>KEY</b><b>NAME</b>
<br></details>

<details>
<summary>In S3 storage class terminology, what does "IA" stand for?</summary>
Infrequent Access
<br></details>

<details>
<summary>Infrequent Access (IA) storage classes are often used for _____ and other old data.</summary>
Backups
<br></details>

<details>
<summary>Cheapest object storage option in AWS</summary>
S3 Glacier Deep Archive
<br></details>

<details>
<summary>S3 Glacier objects are not available for real-time access. They must be _____ before accessing.</summary>
unarchived
<br></details>

<details>
<summary>S3 Glacier expedited retrieval time</summary>
~5 minutes
<br></details>

<details>
<summary>If you manipulate an archived S3 object before the minimum storage duration period, you are billed...</summary>
For the entire minimum storage duration period&nbsp;(90 days Glacier, 180 days Deep Archive)
<br></details>

<details>
<summary>Are all storage classes highly available?</summary>
No,&nbsp;<b>S3 One Zone-IA</b>'s&nbsp;AZ might fail to provide file access.
<br></details>

<details>
<summary>S3 Versioning assigns a&nbsp;version <b>_____&nbsp;</b>for an object to distinguish it from other versions of the same key</summary>
ID
<br></details>

<details>
<summary>The "_____ Object" request permission allows uploading to a bucket.</summary>
<b>PUT</b>
<br></details>

<details>
<summary>S3 Policies are evaluated by creating a list of policies from _____&nbsp;at run-time.</summary>
resource-based permissions and IAM policies
<br></details>

<details>
<summary>Resource policies are applied on...</summary>
A resource
<br></details>

<details>
<summary>Largest filesize that can exist on S3</summary>
5TB
<br></details>

<details>
<summary>A Glacier Archive's maximum total size</summary>
4TB
<br></details>

<details>
<summary>S3 SSE-C stands for...</summary>
<b>S</b>erver-<b>S</b>ide <b>E</b>ncryption&nbsp;with <b>C</b>ustomer-provided keys
<br></details>

<details>
<summary>S3 SSE-KMS stands for...</summary>
<b>S</b>erver-<b>S</b>ide <b>E</b>ncryptionwith CMKs stored in AWS <b>KMS</b>
<br></details>

<details>
<summary>Where can you find when an S3 Object was last modified?</summary>
The object's metadata
<br></details>

<details>
<summary>You can use IAM to grant individual access to individual objects using object _____</summary>
tags
<br></details>

<details>
<summary>To manage a browser's JavaScript GET requests to S3 hosted websites (e.g. to load web fonts from a bucket), you can use...</summary>
CORS (Cross-Origin Resource Sharing)
<br></details>

<details>
<summary>S3 RRS stands for...</summary>
Reduced Redundancy Storage
<br></details>

<details>
<summary>The S3 storage class that automatically selects the cost-effective storage class for objects, with no fee for selection but extra fees for analysing usage is _____</summary>
S3 Intelligent-Tiering
<br></details>

<details>
<summary>The two S3 storage classes intended&nbsp;for infrequent access are...</summary>
S3 Standard-IA
S3 One Zone-IA
<br></details>

<details>
<summary>Can public bucket objects have their ACLs anonymously modified?</summary>
Yes!!! Prevent this by using&nbsp;<b>S3 Block Public Access&nbsp;</b>to disable public write access
<br></details>

<details>
<summary>You can analyze S3 ACLs and policies using...</summary>
S3 Access Analyzer
<br></details>

<details>
<summary>A Glacier archive can have up to _____ archives</summary>
unlimited
<br></details>

<details>
<summary>Can you upload directly to Glacier?</summary>
Yes - via the API
<br></details>

<details>
<summary>How do S3 uploads resume?</summary>
on failure
<br></details>

<details>
<summary>S3 SSE-S3 stands for...</summary>
<b>S</b>erver-<b>S</b>ide <b>E</b>ncryption&nbsp;with <b>S</b>3-Managed Keys
<br></details>

<details>
<summary>Can S3 Buckets be used for access control?</summary>
Yes
<br></details>

<details>
<summary>Can S3 Buckets be used to identify owners of files?</summary>
Yes
<br></details>

<details>
<summary>Can you add custom name-value pairs to an S3 Object's metadata?</summary>
Yes
<br></details>

<details>
<summary>Does an S3 Object's metadata include HTTP metadata?</summary>
Yes - such as Content-Type.
<br></details>

<details>
<summary>Is S3 Intelligent-Tiering a good solution for Data Lakes?</summary>
Yes
<br></details>

<details>
<summary>How can you ensure compliance in S3?</summary>
S3 Object Lock
<br></details>

<details>
<summary>Can an S3 bucket be configured as a failover endpoint?</summary>
Yes - if it is web-enabled.
<br></details>

<details>
<summary>The AWS service designed for long term data archival is...</summary>
S3 Glacier
<br></details>

<details>
<summary>Can you mount a new EBS to an EC2 instance manually via SSH'ing into it?</summary>
Yes
<br></details>

<details>
<summary>Do Infrequent Access (IA) storage classes come with slow data retrieval?</summary>
<b>No!</b>&nbsp;It is&nbsp;still counted in miliseconds.
<br></details>

<details>
<summary>The _____ storage class stores infrequently accessed data across multiple AZ's.</summary>
S3 Standard-IA
<br></details>

<details>
<summary>Can you attach an EBS volume to more than one EC2 instance at the same time?</summary>
No
<br></details>

<details>
<summary>Amazon S3 is a _____ Based Storage solution.</summary>
Object
<br></details>

<details>
<summary>To move an EBS volume to a different AZ, you could create a _____ and recreate it in the new AZ.</summary>
Snapshot
<br></details>

<details>
<summary>EBS <i>resource level permissions</i> are ____, ___ and ____</summary>
ATTACH, DETACH, DELETE
<br></details>

<details>
<summary>_____ storage is a type of storage used for data on persistent disks, such as SSDs and HDDs. File systems and databases make use of it.</summary>
Block
<br></details>

<details>
<summary>Storage Classesfor frequently accessed objects</summary>
S3 Standard
RRS (Reduced Redundancy)
<br></details>

<details>
<summary>Can you create an EBS-backed AMI?</summary>
Yes
<br></details>

<details>
<summary>How are EBS Snapshots backed up to S3?</summary>
Incrementally
<br></details>

<details>
<summary>If you terminate an EC2 instance, would its EBS volume remain?</summary>
Only if instructed to during creation.
<br></details>

<details>
<summary>Are Amazon's EBS volumes encrypted by default?</summary>
No
<br></details>

<details>
<summary>If an Amazon EBS volume is the root device of an instance, can I detach it without stopping the instance?</summary>
No
<br></details>

<details>
<summary>What does EBS stand for?</summary>
Elastic Block Storage
<br></details>

<details>
<summary>In S3, can you can have events that trigger notifications?</summary>
Yes
<br></details>

<details>
<summary>Is enabling versioning on a bucket permanent?</summary>
Yes
<br></details>

<details>
<summary>When an EC2 instance's network throughput towards an EBS volume is prioritized, that instance is called _____</summary>
EBS Optimized
<br></details>

<details>
<summary>Is data on S3 Standard considered successfully stored once uploaded to a single AZ?</summary>
No - you don't get a success until it is replicated across AZs
<br></details>

<details>
<summary>If an Amazon EBS volume is not the root volume, can you detach it without stopping the instance?</summary>
Yes
<br></details>

<details>
<summary>Can you create your own RAID 0/5/10 with EBS volumes?</summary>
Yes
<br></details>

<details>
<summary>In order to enable encryption at rest using EC2 and Elastic Block Store you need to configure encryption when _____ the EBS volume.</summary>
creating
<br></details>

<details>
<summary>Does an EBS volume have to be in the same AZ as an EC2 instance it attaches to?</summary>
Yes
<br></details>

<details>
<summary>Are Storage Gateway copies up to S3 synchronous?</summary>
No - Asynchronous
<br></details>

<details>
<summary>EBS data is redundantly stored in multiple physical locations within the same _____</summary>
Availability Zone
<br></details>

<details>
<summary><b>S3 Transfer Acceleration</b> is...</summary>
CDN-accelerated premium long-distance transfer service
global customers uploading to one bucket&nbsp;
transfering large data across continents
when unable to utilize all available bandwidth when uploading to S3
<br></details>

<details>
<summary>You are hosting the website "example.com" in eu-west-1. There is a static DR site available on S3 in the event that the primary site would go down, and the bucket name is called “examplecom”. The static website's S3 URL would be https://_____.s3-website-_____.amazonaws.com</summary>
https://examplecom.s3-website-eu-west-1.amazonaws.com
<br></details>

<details>
<summary>Is S3 a durable key-value store?</summary>
Yes
<br></details>

<details>
<summary>EBS volume data is replicated across multiple servers <i>in a single _____</i>&nbsp;to prevent the loss of data from the failure of any single component.&nbsp;</summary>
&nbsp;Availability Zone
<br></details>

<details>
<summary>An EBS volume is stored in a single _____, meaning it cannot tolerate its failure.</summary>
Availability Zone
<br></details>

<details>
<summary>Do the Amazon EBS volumes persist independently from the running life of an Amazon EC2 instance?</summary>
Yes
<br></details>

<details>
<summary>Is S3 storage structure hierarchical?</summary>
No - you can make your own prefixes to make it appear so however.
<br></details>

<details>
<summary>Can you create regional buckets?</summary>
Yes
<br></details>

<details>
<summary>Objects consist of two parts:</summary>
Object data
Metadata
<br></details>

<details>
<summary>Can <b>GET </b>requests<b>&nbsp;</b>return<b>&nbsp;</b>data that is currently still being uploaded?</summary>
No
<br></details>

<details>
<summary>Can you lock S3 objects for concurrent operations?</summary>
No - use a database instead. Or hack it with tags.
<br></details>

<details>
<summary>From within AWS, can you make the update of one key depend on the update of another key?</summary>
No
<br></details>

<details>
<summary>Default Encryption is enabled for a replication destination bucket
What happens depending on whether the objects in the source bucket are encrypted?</summary>
<b>unencrypted</b>destination files are encrypted with the destination bucket's default encryption
<b>encrypted</b>the same encryption is used at the destination
<br></details>

<details>
<summary>To be able to recreate an EBS volume at a later date, a _____ can be stored.</summary>
snapshot of it
<br></details>

<details>
<summary>In S3, should you store notifications?</summary>
No
<br></details>

<details>
<summary>There are no transfer costs from EC2 to S3 within the same _____</summary>
region
<br></details>

<details>
<summary>S3 website hosting URL format is _____.s3.-website-_____.amazonaws.com</summary>
<b>BUCKETNAME</b>.s3-website-<b>REGION</b>.amazonaws.com
<br></details>

<details>
<summary>Are Instance store volumes faster than EBS?</summary>
Yes.&nbsp;
<br></details>

<details>
<summary>In S3, is data encrypted at rest decrypted as it is sent to the customer at download?</summary>
Yes
<br></details>

<details>
<summary>A named, uniquely-addressable,&nbsp;regional S3 Glacier archive container is called a...</summary>
Vault
<br></details>

<details>
<summary>Amazon EBS snapshots are compressed and updated ____, so the storage used in any snapshot is generally much less than the storage consumed on an Amazon EBS volume.&nbsp;</summary>
incrementally
<br></details>

<details>
<summary>Can an instance store volume be detached/reattached from an EC2 instance?</summary>
No
<br></details>

<details>
<summary>What 2 things can you do together to protect objects in a bucket from being accidentally overwritten or deleted.</summary>
Enable bucket versioning and MFA delete
<br></details>

<details>
<summary>Can you restrict access to an S3 bucket by date?</summary>
Yes
<br></details>

<details>
<summary>You can enforce that only encrypted objects be uploaded to your S3 bucket via _____</summary>
bucket policy
<br></details>

<details>
<summary>Is S3 considered a durable key-value store?</summary>
Yes
<br></details>

<details>
<summary>When you view the block device mapping for your EC2 instance, can you see the instance store volumes?</summary>
No
<br></details>

<details>
<summary>A snapshot's status is considered _____ until it is complete.</summary>
pending
<br></details>

<details>
<summary>Do Bucket names have to be regionally unique?</summary>
Yes
<br></details>

<details>
<summary>In an S3 "requester pays" bucket, who pays for the <b>storing </b>of data?</summary>
The owner
<br></details>

<details>
<summary>What user are unauthenticated requests made by?</summary>
the <b>anonymous </b>user, ACL ID&nbsp;<b>65a011a29cdf8ec533ec3d1ccaae921c</b>
<br></details>

<details>
<summary>Is the namespace of buckets shared and global among all AWS users?</summary>
Yes
<br></details>

<details>
<summary>Are buckets associated with a region?</summary>
Yes
<br></details>

<details>
<summary>EBS volumes behave like raw, unformatted, external block devices that atach to _____</summary>
EC2 instances
<br></details>

<details>
<summary>Are snapshots updated incrementally?</summary>
Yes
<br></details>

<details>
<summary>Where are EBS Snapshots stored?</summary>
S3
<br></details>

<details>
<summary>In S3, should you store your website database?</summary>
No
<br></details>

<details>
<summary>Does Glacier cost around a penny per GB?</summary>
Yes
<br></details>

<details>
<summary>I/O size is capped at 256 KiB for _____ volumes and 1,024 KiB for ____ volumes</summary>
SSD&nbsp;
magnetic
<br></details>

<details>
<summary>When you provision IOPS, you're not guaranteed to get that much throughput from the EC2 instance it's attached to, but it guarantees that the volume can _____</summary>
handle that much IOPS. You still might need to use EBS Optimization, a larger instance size or a network optimized instance.
<br></details>

<details>
<summary>An EBS volume can be configured as encrypted at-rest, but the encryption/decryption actually happens on _____ and then copied encrypted to the EBS volume.</summary>
its EC2 instance
<br></details>

<details>
<summary>Instance store volumes are acceptable when storing _____ data, or synchronizing data between multiple server for _____</summary>
temporary
fault-tolerance
<br></details>

<details>
<summary>What does CORS stand for?</summary>
Cross Origin Resource Sharing
<br></details>

<details>
<summary>_____ allows to integrate on-premises IT environments with cloud storage</summary>
AWS Storage Gateway
<br></details>

<details>
<summary>To prevent the deletion of EBS volumes created and attached to an instance at launch when the instance is terminated, you can modify the _____ instance launch flag.</summary>
DeleteOnTermination
<br></details>

<details>
<summary>Does disabling automated backups also disable point-in-time recovery?</summary>
Yes
<br></details>

<details>
<summary>Can I delete a snapshot of the root device of an EBS volume used by a registered AMI?</summary>
Yes
<br></details>

<details>
<summary>Fundamental container for data storage</summary>
Bucket
<br></details>

<details>
<summary>How could you encrypt some already existing Amazon S3 objects?</summary>
<b>S3 batch operations </b>
<br></details>

<details>
<summary>Named, configurable network endpoints attachable to S3 Buckets are called...</summary>
Access points
<br></details>

<details>
<summary>Can you create an Access Point for someone else's bucket?</summary>
No
<br></details>

<details>
<summary><b>Storage Classes</b>List all 7 storage classes</summary>
S3 StandardS3 Standard-IAS3 One Zone-IA
S3 GlacierS3 Glacier Deep Archive
S3 Intelligent-Tiering
RRS (not recommended)
<br></details>

<details>
<summary>In<b> S3 Batch Operations, </b>an API action such as copying objects is called a...</summary>
Operation
<br></details>

<details>
<summary>The recommended storage service for a database is...</summary>
EBS
<br></details>

<details>
<summary>Can the snapshots with AWS Marketplace product codes be made public?</summary>
No
<br></details>

<details>
<summary>Can you have provisioned IOPS with your EBS volumes?</summary>
Yes
<br></details>

<details>
<summary>Are snapshots encrypted automatically?</summary>
No
<br></details>

<details>
<summary>Can you manage Lifecycle of objects based on their tags?</summary>
Yes
<br></details>

<details>
<summary>What service can be used to quickly import external data to S3?</summary>
Snowball
<br></details>

<details>
<summary>_____ upload is required for objects larger than 5GB.</summary>
Multipart
<br></details>

<details>
<summary>Are you charged full for each EBS snapshot?</summary>
No - only for total storage used, as snapshots are incremental.
<br></details>

<details>
<summary>Why might a bucket not show up in your list of available endpoints?</summary>
Bucket is web-disabled
<br></details>

<details>
<summary>Are you charged by number of requests to your S3 files?</summary>
Yes
<br></details>

<details>
<summary>How does S3 high availability work?</summary>
Data is eventually replicated across multiple data center servers
<br></details>

<details>
<summary>An object you uploaded is missing from the list. Why?</summary>
It might not have been replicated to your location yet.
<br></details>

<details>
<summary>S3 Bucket Request Authorization Flow Diagram</summary>
<img src="AccessControlAuthorizationFlowBucketResource.png">
<br></details>

<details>
<summary>In <b>S3 Batch Operations,&nbsp;</b>a job's unit of execution over a single object (such as an API call) is called a...</summary>
Task
<br></details>

<details>
<summary>An EC2 instance terminates. Is all of the instance's local data on the hard drive deleted?</summary>
Yes
<br></details>

<details>
<summary>Can you set different IAM permissions to S3 Objects based on their tags?</summary>
Yes
<br></details>

<details>
<summary>You upload a file to S3 after enabling default encryption.
What happens depending on whether you've included encryption information in the header?</summary>
<b>no header</b>bucket default encryption is used
<b>encryption header</b>header encryption is used
<br></details>

<details>
<summary>A request is made using <b>root credentials</b> of AWS account 1111-1111-1111 for a bucket operation owned by AWS account 2222-2222-2222. No IAM users are involved in this request.&nbsp;Because the request is made using root credentials of an AWS account, the&nbsp;<b>user context&nbsp;</b>is _____.&nbsp;In the&nbsp;<b>bucket context</b>, Amazon S3 examines _____. If the bucket owner (AWS account 2222-2222-2222) has not authorized AWS account 1111-1111-1111 to perform the requested operation, Amazon S3 denies the request.</summary>
ignored
the bucket policy

<img src="example20-policy-eval-logic.png">
<br></details>

<details>
<summary>A request is sent by Jill, an IAM user in AWS account 1111-1111-1111, which also owns the bucket. Because the request is from an IAM principal, in the&nbsp;<b>user context</b>, Amazon S3 evaluates all policies that belong to the parent AWS account to determine if Jill has permission to perform the operation. In this example, parent AWS account 1111-1111-1111, to which the principal belongs, is also the bucket owner. As a result, in addition to the user policy, Amazon S3 also evaluates the bucket policy and bucket ACL in the same context, because they belong to the same account.&nbsp;Because Amazon S3 evaluated the bucket policy and bucket ACL as part of the&nbsp;<b>user context</b>, it does not evaluate the&nbsp;<b>_____</b>.</summary>
<b>bucket context</b><b>
</b><img src="example30-policy-eval-logic.png"><b>
</b>
<br></details>

<details>
<summary>A request is sent by Jill, an IAM user whose parent AWS account is 1111-1111-1111, but the bucket is owned by another AWS account, 2222-2222-2222.&nbsp;Because the request is from an IAM principal, Amazon S3 evaluates the _____&nbsp;by reviewing the policies authored by the account to verify that Jill has the necessary permissions. If Jill has permission, then Amazon S3 moves on to evaluate the <b>bucket context</b>; if not, it denies the request. In the <b>bucket context</b>, Amazon S3 verifies that bucket owner 2222-2222-2222 has granted Jill (or her parent AWS account) permission to perform the requested operation. If she has that permission, Amazon S3 grants the request and performs the operation.</summary>
<b>user context</b>

<img src="example40-policy-eval-logic.png">
<br></details>

<details>
<summary>Can Lifecycle policies target folders?</summary>
Yes
<br></details>

<details>
<summary>To determine whether the requester has permission to perform an operation, S3 considers the following contexts, in order: _____, _____, _____</summary>
User, Bucket, Object&nbsp;
<br></details>

<details>
<summary>Object Operation authentication flow</summary>
User Context &gt; Bucket Context &gt; Object Context

<img src="AccessControlAuthorizationFlowObjectResource.png">
<br></details>

<details>
<summary>The bucket owner sends a request for a bucket operation using the <b>root credentials</b> of the AWS account.&nbsp;Because the request is made by using root credentials of an AWS account, the&nbsp;<b>user context</b>&nbsp;is _____.&nbsp;In the&nbsp;<b>bucket context</b>, Amazon S3 reviews _____. Amazon S3 authorizes the request.</summary>
ignored
the bucket policy, to determine if the requester has permission to perform the operation

<img src="example10-policy-eval-logic.png">
<br></details>

<details>
<summary>IAM user Jill, whose parent AWS account is 1111-1111-1111, sends an object operation request (for example, Get object) for an object owned by AWS account 3333-3333-3333 in a bucket owned by AWS account 2222-2222-2222. Jill will need permission from the parent AWS account, the bucket owner, and the object owner. Because the request is from an IAM principal, Amazon S3 evaluates the user context to verify that the parent AWS account 1111-1111-1111 has given Jill permission to perform the requested operation. If she has that permission, Amazon S3 evaluates the bucket context. Otherwise, Amazon S3 denies the request. In the bucket context, the bucket owner, AWS account 2222-2222-2222, is the context authority. Amazon S3 evaluates the bucket policy to determine if the bucket owner has explicitly denied Jill access to the object. In the object context, the context authority is AWS account 3333-3333-3333, the object owner. Amazon S3 evaluates the object ACL to determine if Jill has permission to access the object. If she does, Amazon S3 authorizes the request.</summary>
User Context &gt; Bucket Context &gt; Object Context
<img src="example50-policy-eval-logic.png">
<br></details>

<details>
<summary>An EC2 instance terminates. What happens to any EBS volumes attached to it?</summary>
They are preserved - except the OS volume.
<br></details>

<details>
<summary>If I want to run a database on an EC2 instance, which is the most recommended Amazon storage option?</summary>
EBS
<br></details>

<details>
<summary>The max number of S3 buckets you can have in your account by default is...</summary>
100
<br></details>

<details>
<summary>The S3 "Infrequent Access" storage class requires a minimum object size of?</summary>
128KB
<br></details>

<details>
<summary>Are Server-Side encryption options mutually exclusive?</summary>
Yes
<br></details>

<details>
<summary>Why choose a Region for an S3 bucket?</summary>
Cost
Latency
Law
<br></details>

<details>
<summary>Two PUT requests are simultaneously made to an object. What happens?</summary>
The latest timestamp wins, older is ignored.
<br></details>

<details>
<summary>S3 Default EncryptionDoes it retroactively re-encrypt previously existing objects?</summary>
No
<br></details>

<details>
<summary>Fundamental entity stored in S3</summary>
Objects
<br></details>

<details>
<summary>If you upload an object using an IAM user/role, do the objects belong to the bucket owner?</summary>
No - to the user/role
<br></details>

<details>
<summary>When using versioning on a bucket, the latest version of the object called the _____ version.</summary>
Live
<br></details>

<details>
<summary>A glacier job typically completes in how much time?</summary>
3-5 hours
<br></details>

<details>
<summary>An on-premise virtual appliance that can be used to cache S3 locally at a customers site is called...</summary>
AWS Storage Gateway
<br></details>

<details>
<summary>Can S3 endpoints be accessed across a VPC peering connection?</summary>
No
<br></details>

<details>
<summary>Can S3 version its objects?</summary>
Yes
<br></details>

<details>
<summary>With S3 versioning, do you pay for the space required for every version of a file kept?</summary>
Yes
<br></details>

<details>
<summary>An S3 object can be as small as ____</summary>
0Bytes
<br></details>

