# Integration 

<details>
<summary>What does Amazon SWF stand for?</summary>
Simple Work Flow
<br></details>

<details>
<summary>Your website has premium and free tier members, whose actions are stored in SQS. How can you ensure your premium members have higher priority in your app?</summary>
Create one premium tier SQS queue and one free tier SQS queue, then have your app prioritize the actions stored in the premium queue - once it is empty, start working on the free tier queue.
<br></details>

<details>
<summary>SWF helps users coordinate synchronous and asynchronous _____&nbsp;</summary>
tasks
<br></details>

<details>
<summary>SQS can retain stored messages for up to _____</summary>
2 weeks (4 days by default)
<br></details>

<details>
<summary>SQS long polling can wait up to _____</summary>
20 seconds
<br></details>

<details>
<summary>Can SWF create EC2 instances for certain steps?</summary>
Yes
<br></details>

<details>
<summary>Does SQS guarantee no duplicate messages sent?</summary>
No
<br></details>

<details>
<summary>Is an ARN (Amazon Resource Name) created upon creating an SNS topic?</summary>
Yes
<br></details>

<details>
<summary>SNS is a service used for _____</summary>
push notifications
<br></details>

<details>
<summary>SQS visibility timeout can be up to ____</summary>
12 hours
<br></details>

<details>
<summary>S3 Event Notifications events can be sent to _____, _____, _____.</summary>
SNS, SQS, Lambda
<br></details>

<details>
<summary>Is Lambda a valid SNS subscriber?</summary>
Yes
<br></details>

<details>
<summary>Are you charged for polling requests?</summary>
Yes
<br></details>

<details>
<summary>Could you use SWF for a video encoding application, where encoding is done in a number of pre-defined steps?</summary>
Yes
<br></details>

<details>
<summary>Could you use SWF for an application which requires co-ordination between different tasks?</summary>
Yes
<br></details>

<details>
<summary>You can decouple your infrastructure using messaged based queues via _____</summary>
SQS
<br></details>

<details>
<summary>Does SQS guarantee a message will be delivered at least once?</summary>
Yes
<br></details>

<details>
<summary>Does SWF ensure that a task is assigned only once and is never duplicated?</summary>
Yes
<br></details>

<details>
<summary>How could CloudWatch send an alert regarding the billing metrics of an EC2 Instance?</summary>
With SNS (Simple Notification Service)
<br></details>

<details>
<summary>SWF workflows have tasks of type ____ and ____</summary>
Activity and Decision
<br></details>

<details>
<summary>In SWF, a Domain is a collection of related _____</summary>
Workflows
<br></details>

<details>
<summary>SQS is message system that requires worker nodes to poll the _____.</summary>
queue
<br></details>

<details>
<summary>Is SQS a valid SNS subscriber?</summary>
Yes
<br></details>

<details>
<summary>Is e-mail or SMS a valid SNS subscriber?</summary>
Yes
<br></details>

<details>
<summary>Can users be set as SWF "workers" and "deciders"?&nbsp;</summary>
Yes
<br></details>

<details>
<summary>Using SQS, higher receive performance can be achieved by requesting multiple&nbsp;messages in a single _____</summary>
call
<br></details>

<details>
<summary>You need to process a queue of messages where each message is a task that needs to be completed. This can be achieved via _____</summary>
SQS
<br></details>

