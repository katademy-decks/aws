<details>
	<summary>
		You cannot import _____ keys into AWS KMS.
	</summary>
		asymmetric
</details>

<details>
	<summary>
		Logs in AWS _____ will show all AWS KMS API requests, including management and cryptographic requests.
	</summary>
		CloudTrail
</details>

<details>
	<summary>
		AWS CloudHSM also logs all API activity to AWS CloudTrail (cluster / HSM deletions and creations). Each cluster also has its own local logs to record user and key management activity. Each CloudHSM instance also copies the local user and key management activity logs to AWS _____.
	</summary>
		CloudWatch
</details>

<details>
	<summary>
		_____ customer managed CMKs can only be generated within AWS KMS HSMs and there is no option for automatic key rotation.
	</summary>
		Asymmetric
</details>

<details>
	<summary>
		Customer-managed Customer Master Keys which are symmetric, allow defining their key _____, e.g. generated in AWS KMS, generated in AWS CloudHSM, or custom.
	</summary>
		material
</details>

<details>
	<summary>
		When creating an asymmetric CMK, you must specify whether the key can be used for _____ or sign operations, but not both.
	</summary>
		decrypt
</details>

<details>
	<summary>
		Automatic key rotation is unsupported for _____ CMKs. Manually rotate them by creating a new CMK, then mapping an existing key alias from the old CMK to the new CMK.
	</summary>
		asymmetric
</details>

<details>
	<summary>
		When creating an _____ CMK, you must specify whether the key can be used for decrypt or sign operations, but not both.
	</summary>
		asymmetric
</details>

<details>
	<summary>
		Only _____ CMKs can be stored and managed in an AWS KMS custom key store.
	</summary>
		customer managed
</details>

<details>
	<summary>
		Automatic key rotation is not supported for imported keys, _____ keys, or keys generated in an AWS CloudHSM cluster using the AWS KMS custom key store feature.
	</summary>
		asymmetric
</details>

<details>
	<summary>
		Automatic key rotation is unsupported for asymmetric CMKs. Manually rotate them by creating a new CMK, then _____.
	</summary>
		mapping an existing key alias from the old CMK to the new CMK
</details>

<details>
	<summary>
		You can import _____ keys into KMS.
	</summary>
		symmetric
</details>

<details>
	<summary>
		You cannot import key material into a _____ key store and you cannot have AWS KMS automatically rotate keys.
	</summary>
		custom
</details>

<details>
	<summary>
		Automatic key rotation is not supported for imported keys, asymmetric keys, or keys generated in _____.
	</summary>
		an AWS CloudHSM cluster using the AWS KMS custom key store feature
</details>

<details>
	<summary>
		When creating an asymmetric CMK, you must specify whether the key can be used for decrypt or _____ operations, but not both.
	</summary>
		sign
</details>

<details>
	<summary>
		You start using AWS KMS by configuring a CMK, its lifecycle and who can use it to _____.
	</summary>
		sign, encrypt or decrypt data
</details>

<details>
	<summary>
		AWS _____ allows you to encrypt or digitally sign data within your applications.
	</summary>
		KMS
</details>

<details>
	<summary>
		You start using AWS KMS by configuring a _____, its lifecycle and who can use it to sign, encrypt or decrypt data.
	</summary>
		CMK
</details>

<details>
	<summary>
		Customer-managed Customer Master Keys which are symmetric, allow defining their key material, e.g. generated in AWS KMS, generated in AWS _____, or custom.
	</summary>
		CloudHSM
</details>

<details>
	<summary>
		AWS-managed CMKs are always generated and stored in the AWS KMS _____ key store.
	</summary>
		default
</details>

<details>
	<summary>
		Automatic key rotation is not supported for _____ keys, asymmetric keys, or keys generated in an AWS CloudHSM cluster using the AWS KMS custom key store feature.
	</summary>
		imported
</details>

<details>
	<summary>
		_____ CMKs are always generated and stored in the AWS KMS default key store.
	</summary>
		AWS-managed
</details>

<details>
	<summary>
		Customer-managed Customer Master Keys which are _____, allow defining their key material, e.g. generated in AWS KMS, generated in AWS CloudHSM, or custom.
	</summary>
		symmetric
</details>

<details>
	<summary>
		You can provide a specific _____ CMK to an AWS service to encrypt data on your behalf with. You define the access control and usage policy for each _____ CMK.
	</summary>
		customer managed
</details>

<details>
	<summary>
		If you choose to have AWS KMS _____ rotate keys, you don’t have to re-encrypt your data after rotation.
	</summary>
		automatically
</details>

<details>
	<summary>
		AWS CloudHSM also logs all API activity to AWS _____ (cluster / HSM deletions and creations). Each cluster also has its own local logs to record user and key management activity. Each CloudHSM instance also copies the local user and key management activity logs to AWS CloudWatch.
	</summary>
		CloudTrail
</details>

<details>
	<summary>
		Customer-managed Customer Master Keys which are symmetric, allow defining their key material, e.g. generated in AWS _____, generated in AWS CloudHSM, or custom.
	</summary>
		KMS
</details>

<details>
	<summary>
		You cannot use the AWS KMS custom key store functionality with _____ keys.
	</summary>
		asymmetric
</details>

<details>
	<summary>
		AWS CloudHSM also logs all API activity to AWS CloudTrail (cluster / HSM deletions and creations). Each cluster also has its own _____ to record user and key management activity. Each CloudHSM instance also copies the local user and key management activity logs to AWS CloudWatch.
	</summary>
		local logs
</details>

<details>
	<summary>
		You can provide a specific _____ CMK to an AWS service to encrypt data on your behalf with. You define the access control and usage policy for each _____ CMK.
	</summary>
		customer managed
</details>

