# Databases 

<details>
<summary>The AWS DB platforms most suitable for online transaction processing are _____ and _____</summary>
RDS and DynamoDB
<br></details>

<details>
<summary>In RDS when using multiple availability zones, can you use the secondary database as an independent read node?</summary>
No
<br></details>

<details>
<summary>The maximum RDS backup retention period is _____ days.</summary>
35 Days
<br></details>

<details>
<summary>In order to see free memory in RDS metrics, you need to enable _____</summary>
Enhanced monitoring
<br></details>

<details>
<summary>Does installing patches require taking an RDS instance offline?</summary>
Yes
<br></details>

<details>
<summary>In elasticache you can <i>snapshot</i> only ___ engine clusters.</summary>
Redis
<br></details>

<details>
<summary>In a Multi-AZ deployment, Amazon RDS automatically switches to the standby replica if your primary DB Instance has failed by changing the ______ DNS record of the main DB Instance to point to the standby DB Instance.</summary>
CNAME
<br></details>

<details>
<summary>If you modify a DB Instance or the DB parameter group associated with the instance, when do the changes take effect?</summary>
After reboot
<br></details>

<details>
<summary>The AWS service best suited for non relational databases is _____</summary>
DynamoDB
<br></details>

<details>
<summary>Amazon's Elasticache uses the _____ and _____ engines.</summary>
Redis &amp; Memcached
<br></details>

<details>
<summary>Is DynamoDB data automatically replicated across multiple availability zones?</summary>
Yes
<br></details>

<details>
<summary>Are RDS read replicas synchronous or asynchronous?</summary>
Asynchronous
<br></details>

<details>
<summary>Can you initiate a manual reboot with failover in RDS?</summary>
Yes
<br></details>

<details>
<summary>To rebuild and index in RDS without affecting performance, you could do it on a _____ and then promote it to _____</summary>
read replica
primary
<br></details>

<details>
<summary>What's the limit on the amount of data&nbsp;DynamoDB can store?</summary>
None
<br></details>

<details>
<summary>Does Redshift automatically scale up to meet demand?</summary>
No
<br></details>

<details>
<summary>Can RedShift load data from DynamoDB?</summary>
Yes
<br></details>

<details>
<summary>When reading data from Amazon DynamoDB, can users specify whether they want the read to be eventually consistent or strongly consistent?</summary>
Yes
<br></details>

<details>
<summary>Can you have provisioned IOPS for your RDS database?</summary>
Yes
<br></details>

<details>
<summary>Manually created DB Snapshots are _____ after the DB Instance is deleted.</summary>
retained
<br></details>

<details>
<summary>The AWS service used for Business Intelligence Tools/Data Warehousing is _____</summary>
Redshift
<br></details>

<details>
<summary>When doing online transaction processing in RDS, you could use _____ over standard storage.</summary>
provisoned IOPS&nbsp;
<br></details>

<details>
<summary>When do changes to the RDS backup window take effect?</summary>
Immediately
<br></details>

<details>
<summary>Does DynamoDB scale and is fault tolerant automatically?</summary>
Yes
<br></details>

<details>
<summary>RedShift is for _____ big data.</summary>
Data warehousing
<br></details>

<details>
<summary>In RDS, can you change the disk type without any downtime?</summary>
Yes - if multi-AZ.
<br></details>

<details>
<summary>Can you promote an RDS read replica to a primary instance?</summary>
Yes
<br></details>

<details>
<summary>Does RDS supports MySQL clustering?</summary>
No
<br></details>

<details>
<summary>With Redis Elasticache you can have up to __ read replicas in different AZ's</summary>
5
<br></details>

<details>
<summary>Using _____ for your web application cache can reduce the load on your database and web servers.</summary>
Elasticache&nbsp;
<br></details>

<details>
<summary>Are standby RDS instances in the same Region as the primary?</summary>
Yes
<br></details>

<details>
<summary>Is a standby RDS instance in the same Availability Zone as the primary?</summary>
No
<br></details>

<details>
<summary>AWS service health can be chcked at https://_____.aws.amazon.com</summary>
https://status.aws.amazon.com
<br></details>

<details>
<summary>How does AWS RDS fail-over?</summary>
Route 53 changes the DNS
<br></details>

<details>
<summary>Can RedShift load data from S3?</summary>
Yes
<br></details>

<details>
<summary>Can you create RDS read replicas for read-heavy applications?</summary>
Yes
<br></details>

<details>
<summary>Are DynamoDB costs, among other things, based on in/out data transfer per month?</summary>
Yes
<br></details>

<details>
<summary>In the event of a cache node failure, the Elasticache&nbsp;cluster remains available, but _____ may be reduced until the new cache node is populated.</summary>
performance
<br></details>

<details>
<summary>RDS DB snapshots and automated backups are stored in _____</summary>
S3
<br></details>

<details>
<summary>Does RDS automatically backup daily?</summary>
Yes
<br></details>

<details>
<summary>Can RDS tolerate an Availability Zone failure?</summary>
Yes if deployed Multi-AZ.
<br></details>

<details>
<summary>Does Multi-AZ RDS make the database more available during maintenance tasks?</summary>
Yes
<br></details>

<details>
<summary>Are DynamoDB costs, among other things, based on provisioned throughput capacity?</summary>
Yes
<br></details>

<details>
<summary>What AWS services can you use to store session data?</summary>
RDS, DynamoDB &amp; Elasticache.
<br></details>

<details>
<summary>Which AWS services could you use to cache database queries?</summary>
CloudFront
Amazon Elastic Cloud
<br></details>

<details>
<summary>Are DynamoDB costs, among other things, based on the Indexed Data Storage?</summary>
Yes
<br></details>

