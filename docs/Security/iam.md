<details>
	<summary>
		Can you associate an IAM role with an Auto Scaling group? _____
	</summary>
		Yes.
</details>

<details>
	<summary>
		To request temporary security credentials for federated users, call the GetFederationToken, AssumeRole, _____, or AssumeRoleWithWebIdentity AWS STS APIs.
	</summary>
		AssumeRoleWithSAML
</details>

<details>
	<summary>
		Groups can be granted _____ using IAM policies.
	</summary>
		permissions
</details>

<details>
	<summary>
		Can you create multiple access IDs and secret keys for an IAM user? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		IAM policies are attached to _____ to assign permissions to AWS resources.
	</summary>
		users, groups, and roles
</details>

<details>
	<summary>
		Can a temporary security credential be revoked prior to its expiration? _____
	</summary>
		No. You can revoke permissions of the IAM user who requested it instead.
</details>

<details>
	<summary>
		"Temporary security credentials (or ""tokens"") consist of: - an access key ID - a secret access key - a security token - permissions - _____"
	</summary>
		an expiration date
</details>

<details>
	<summary>
		When you request temporary security credentials for your federated user using an AssumeRole API, you can optionally include an access policy with the request. The federated user’s privileges are the intersection of permissions granted by the access policy passed with the request and _____.
	</summary>
		the access policy attached to the assumed IAM role
</details>

<details>
	<summary>
		A service-linked role can be assumed only by the _____.
	</summary>
		linked service
</details>

<details>
	<summary>
		You can use the IAM _____ via AWS SDKs / CLI in addition to the web console. Use the iam:SimulatePrincipalPolicy API to programmatically test existing IAM policies, or iam:SimulateCustomPolicy to test policies that are not yet attached to a user/group/role.
	</summary>
		policy simulator
</details>

<details>
	<summary>
		"Temporary security credentials (or ""tokens"") consist of: - an access key ID - a secret access key - a security token - _____ - an expiration date"
	</summary>
		permissions
</details>

<details>
	<summary>
		_____ allow employees and applications to securely access AWS service APIs without needing to create an AWS identity for them.
	</summary>
		Temporary security credentials
</details>

<details>
	<summary>
		An IAM _____ can belong to multiple IAM groups.
	</summary>
		user
</details>

<details>
	<summary>
		IAM roles are not associated with a specific user or group. Users, applications or AWS services must _____ IAM roles to acquire their permissions.
	</summary>
		assume
</details>

<details>
	<summary>
		Managed policies provides a set of commonly used permissions that you can attach to _____.
	</summary>
		IAM users, groups, and roles
</details>

<details>
	<summary>
		A _____ is a role that delegates permission to manage AWS resources to an AWS service (the linked service).
	</summary>
		service-linked role
</details>

<details>
	<summary>
		"The Administrator Access IAM _____ gives the ""Admins"" group permission to access all account resources."
	</summary>
		policy template
</details>

<details>
	<summary>
		Power User Access grants access to all AWS services except _____
	</summary>
		IAM management
</details>

<details>
	<summary>
		"Temporary security credentials (or ""tokens"") consist of: - an access key ID - _____ - a security token - permissions - an expiration date"
	</summary>
		a secret access key
</details>

<details>
	<summary>
		Root accounts are not bound by _____ policies.
	</summary>
		IAM
</details>

<details>
	<summary>
		Can an IAM role affect multiple EC2 instances? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		AWS permissions are either _____-based and Resource-based
	</summary>
		User
</details>

<details>
	<summary>
		You cannot restrict the temporary security credentials to a particular region or subset of regions, except credentials from _____.
	</summary>
		GovCloud (US) and China (Beijing)
</details>

<details>
	<summary>
		By assuming an _____ with correct permissions, IAM users can access resources in another AWS account.
	</summary>
		IAM role
</details>

<details>
	<summary>
		AWS permissions are either User-based and _____-based
	</summary>
		Resource
</details>

<details>
	<summary>
		Can one IAM role have multiple policies assigned? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Federated users are managed outside of AWS IAM (e.g. in your corporate directory), but are granted access to AWS via _____.
	</summary>
		temporary security credentials
</details>

<details>
	<summary>
		New IAM users have a Access Key ID and _____ automatically generated for them.
	</summary>
		Secret Access Key
</details>

<details>
	<summary>
		_____, when attached to EC2 instances, provide security credentials to use when making requests from running EC2 instances to AWS services.
	</summary>
		IAM roles
</details>

<details>
	<summary>
		You can programmatically request _____ to provide federated users with secure and direct access to AWS APIs.
	</summary>
		temporary security credentials
</details>

<details>
	<summary>
		IAM provides _____ for automatically assigning permissions to groups
	</summary>
		policy templates
</details>

<details>
	<summary>
		A non-root IAM user can be a part of up to _____ groups.
	</summary>
		10
</details>

<details>
	<summary>
		"The _____ IAM policy template gives the ""Admins"" group permission to access all account resources."
	</summary>
		Administrator Access
</details>

<details>
	<summary>
		AWS allows you to use the same _____ security key with several root and IAM users across multiple accounts.
	</summary>
		U2F
</details>

<details>
	<summary>
		You can retrieve IAM Role access keys on an EC2 instance using _____.
	</summary>
		its metadata service
</details>

<details>
	<summary>
		To get a report of credentials in your AWS infrastructure, you could download a Credential Report from _____.
	</summary>
		IAM
</details>

<details>
	<summary>
		You can sign requests made to AWS APIs with the temporary security credentials from AWS _____.
	</summary>
		Security Token Service (STS)
</details>

<details>
	<summary>
		When you request temporary security credentials for your federated user using an AssumeRole API, you can optionally include an access policy with the request. The federated user’s privileges are the intersection of permissions granted by _____ and the access policy attached to the assumed IAM role.
	</summary>
		the access policy passed with the request
</details>

<details>
	<summary>
		An IAM _____ has permanent long-term credentials to access AWS services.
	</summary>
		user
</details>

<details>
	<summary>
		You assume an IAM role by calling the AWS _____ AssumeRole APIs, which return a set of temporary security credentials that applications can use to sign requests to AWS APIs.
	</summary>
		Security Token Service (STS)
</details>

<details>
	<summary>
		IAM manages fine-grained access control to _____.
	</summary>
		AWS resources
</details>

<details>
	<summary>
		Can you set usage quotas on individual IAM users? _____
	</summary>
		No. All limits affect the entire AWS account.
</details>

<details>
	<summary>
		"_____ consist of: - an access key ID - a secret access key - a security token - permissions - an expiration date"
	</summary>
		Temporary security credentials (or ""tokens"")
</details>

<details>
	<summary>
		You assume an IAM role by calling the AWS Security Token Service (STS) _____ APIs, which return a set of temporary security credentials that applications can use to sign requests to AWS APIs.
	</summary>
		AssumeRole
</details>

<details>
	<summary>
		"Can an IAM role make requests to the AWS APIs? _____"
	</summary>
		No. IAM roles are meant to be ""assumed"" by IAM users, applications or AWS services.
</details>

<details>
	<summary>
		EC2 instances should not have AWS API credentials stored on their filesystems. You should be assigning _____.
	</summary>
		roles
</details>

<details>
	<summary>
		IAM actions, STS actions, and AWS sign-ins are logged in AWS _____.
	</summary>
		CloudTrail
</details>

<details>
	<summary>
		Does IAM integrate with Active Directory? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Can an IAM policy specify access to a resource by IP range? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		"Temporary security credentials (or ""tokens"") consist of: - _____ - a secret access key - a security token - permissions - an expiration date"
	</summary>
		an access key ID
</details>

<details>
	<summary>
		An IAM _____ is an IAM entity with permissions for making AWS service requests.
	</summary>
		role
</details>

<details>
	<summary>
		Does IAM allow you to create a password rotation policy? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		By default, IAM _____ have no permissions. Users with sufficient permissions must use a policy to grant them desired permissions.
	</summary>
		users, groups, and roles
</details>

<details>
	<summary>
		You can sign requests made to AWS APIs with the _____ from AWS Security Token Service (STS).
	</summary>
		temporary security credentials
</details>

<details>
	<summary>
		_____ shows the time since an IAM entity last accessed an AWS service. Use this to remove unnecessary permissions.
	</summary>
		IAM console
</details>

<details>
	<summary>
		Can IAM policies restrict by time of day? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		By _____ an IAM role with correct permissions, IAM users can access resources in another AWS account.
	</summary>
		assuming
</details>

<details>
	<summary>
		"Temporary security credentials (or ""tokens"") consist of: - an access key ID - a secret access key - _____ - permissions - an expiration date"
	</summary>
		a security token
</details>

<details>
	<summary>
		Managed policies can only be attached to IAM users, groups, or roles. You cannot use them as _____ policies.
	</summary>
		resource-based
</details>

<details>
	<summary>
		An IAM user can belong to multiple IAM _____.
	</summary>
		groups
</details>

<details>
	<summary>
		An IAM _____ is a collection of IAM users.
	</summary>
		group
</details>

<details>
	<summary>
		Can IAM policies apply to a group? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		A service-linked role can be _____ only by the linked service.
	</summary>
		assumed
</details>

<details>
	<summary>
		IAM _____ delegate access with defined permissions to entities without having to share long-term access keys.
	</summary>
		Roles
</details>

<details>
	<summary>
		What happens after 3 unsuccessful attempts to access an HSM partition with HSM Admin credentials? _____
	</summary>
		The HSM partitions are erased
</details>

<details>
	<summary>
		_____ users are managed outside of AWS IAM (e.g. in your corporate directory), but are granted access to AWS via temporary security credentials.
	</summary>
		Federated
</details>

<details>
	<summary>
		To get a report of credentials in your AWS infrastructure, you could download a _____ from IAM.
	</summary>
		Credential Report
</details>

<details>
	<summary>
		You can use the IAM policy simulator via AWS SDKs / CLI in addition to the web console. Use the iam:_____ API to programmatically test existing IAM policies, or iam:SimulateCustomPolicy to test policies that are not yet attached to a user/group/role.
	</summary>
		SimulatePrincipalPolicy
</details>

<details>
	<summary>
		The isolated cloud for government access only is called _____
	</summary>
		GovCloud
</details>

<details>
	<summary>
		Can groups belong to other groups? _____
	</summary>
		No
</details>

<details>
	<summary>
		ISMS stands for _____. It is a collection of information security policies and processes for your organization’s assets on AWS.
	</summary>
		Information Security Management System
</details>

<details>
	<summary>
		New IAM users have a _____ and Secret Access Key automatically generated for them.
	</summary>
		Access Key ID
</details>

<details>
	<summary>
		_____ provides a set of commonly used permissions that you can attach to IAM users, groups, and roles.
	</summary>
		Managed policies
</details>

<details>
	<summary>
		Can you structure a collection of users in a hierarchical way, like in LDAP? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		IAM manages fine-grained _____ to AWS resources.
	</summary>
		access control
</details>

<details>
	<summary>
		To request temporary security credentials for federated users, call the GetFederationToken, AssumeRole, AssumeRoleWithSAML, or _____ AWS STS APIs.
	</summary>
		AssumeRoleWithWebIdentity
</details>

<details>
	<summary>
		By default, IAM users, groups, and roles have no permissions. Users with sufficient permissions must use a _____ to grant them desired permissions.
	</summary>
		policy
</details>

<details>
	<summary>
		An EC2 instance's temporary security credentials are automatically rotated several times _____.
	</summary>
		per day
</details>

<details>
	<summary>
		When you request _____ for your federated user using an AssumeRole API, you can optionally include an access policy with the request. The federated user’s privileges are the intersection of permissions granted by the access policy passed with the request and the access policy attached to the assumed IAM role.
	</summary>
		temporary security credentials
</details>

<details>
	<summary>
		You can use the IAM policy simulator via AWS SDKs / CLI in addition to the web console. Use the iam:SimulatePrincipalPolicy API to programmatically test existing IAM policies, or iam:_____ to test policies that are not yet attached to a user/group/role.
	</summary>
		SimulateCustomPolicy
</details>

<details>
	<summary>
		To request temporary security credentials for federated users, call the _____, AssumeRole, AssumeRoleWithSAML, or AssumeRoleWithWebIdentity AWS STS APIs.
	</summary>
		GetFederationToken
</details>

<details>
	<summary>
		An IAM group is a collection of IAM _____.
	</summary>
		users
</details>

<details>
	<summary>
		With _____, external identities (from Active Directory, Cognito, Google OR Facebook) can be granted secure access to resources in your AWS account without creating IAM users.
	</summary>
		identity federation
</details>

<details>
	<summary>
		A service-linked role is a role that delegates permission to manage AWS resources to _____.
	</summary>
		an AWS service (the linked service)
</details>

<details>
	<summary>
		Can you enforce Multi-Factor Authentication via an IAM access policy? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		How many MFA devices can a user have in AWS by default? _____
	</summary>
		1
</details>

<details>
	<summary>
		_____ grants access to all AWS services except IAM management
	</summary>
		Power User Access
</details>

<details>
	<summary>
		To request temporary security credentials for federated users, call the GetFederationToken, AssumeRole, AssumeRoleWithSAML, or AssumeRoleWithWebIdentity AWS _____ APIs.
	</summary>
		STS
</details>

<details>
	<summary>
		Groups can be granted permissions using IAM _____.
	</summary>
		policies
</details>

<details>
	<summary>
		An IAM _____ provides a formal statement of one or more permissions.
	</summary>
		Policy
</details>

<details>
	<summary>
		_____ accounts are not bound by IAM policies.
	</summary>
		Root
</details>

<details>
	<summary>
		SAML stands for _____
	</summary>
		Security Assertion Markup Language.
</details>

<details>
	<summary>
		To request temporary security credentials for federated users, call the GetFederationToken, _____, AssumeRoleWithSAML, or AssumeRoleWithWebIdentity AWS STS APIs.
	</summary>
		AssumeRole
</details>

<details>
	<summary>
		IAM's _____ can visualize and test new policies and existing policies attached to users, groups, or roles.
	</summary>
		policy simulator
</details>

<details>
	<summary>
		STS stands for _____. It is the service IAM roles use to rotate credentials.
	</summary>
		Security Token Service
</details>

<details>
	<summary>
		By assuming an IAM role with correct permissions, _____ can access resources in another AWS account.
	</summary>
		IAM users
</details>

<details>
	<summary>
		IAM role credentials are rotated every _____ hours by default
	</summary>
		12
</details>

<details>
	<summary>
		A _____ can be assumed only by the linked service.
	</summary>
		service-linked role
</details>

