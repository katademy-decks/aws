<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. _____ routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The POP returns the file if it's present in its cache. Otherwise, the POP compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the POP forwards the files to the user and caches them for later.
	</summary>
		DNS
</details>

<details>
	<summary>
		A CloudFront Distribution is an invalid endpoint in Route53 until it has a _____ set.
	</summary>
		Alternate Domain Name
</details>

<details>
	<summary>
		When requested content is missing at a CloudFront _____, CloudFront delivers content from the origin and caches it.
	</summary>
		POP (edge location)
</details>

<details>
	<summary>
		When requested content is missing at a CloudFront POP (edge location), CloudFront delivers content from _____ and caches it.
	</summary>
		the origin
</details>

<details>
	<summary>
		Can you invalidate cached content at an edge location? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Modify different CloudFront behaviors like cache timeout by using _____
	</summary>
		Patterns
</details>

<details>
	<summary>
		"You upload files to a CloudFront edge location and have it sync back to the origin by allowing _____ in ""Allowed HTTP Methods"""
	</summary>
		PUT/POST
</details>

<details>
	<summary>
		Can an S3 bucket be used as a CloudFront origin server? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Could you cache database queries in CloudFront? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Signed URLs can be created to access objects on CloudFront edge locations. Policies can specify its expiration (either based on time or number of uses), permitted _____,
	</summary>
		IP addresses
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The POP returns the file if it's present in its _____. Otherwise, the POP compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the POP forwards the files to the user and caches them for later.
	</summary>
		cache
</details>

<details>
	<summary>
		An S3 bucket used as a failover page must have its name match the page's domain name. With AWS _____ you can configure multiple alternate domain names on the distribution.
	</summary>
		CloudFront
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The _____ returns the file if it's present in its cache. Otherwise, the _____ compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the _____ forwards the files to the user and caches them for later.
	</summary>
		POP
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The POP returns the file if it's present in its cache. Otherwise, the POP compares the request with the specifications in your _____ and downloads the missing file from the origin server. Once the first byte arrives from the origin, the POP forwards the files to the user and caches them for later.
	</summary>
		Distribution
</details>

<details>
	<summary>
		Signed URLs are managed by a _____ pair.
	</summary>
		key
</details>

<details>
	<summary>
		Signed URLs can be created to access objects on CloudFront edge locations. Policies can specify its expiration (either based on time or _____), permitted IP addresses,
	</summary>
		number of uses
</details>

<details>
	<summary>
		Signed URLs can be created to access objects on CloudFront edge locations. Policies can specify its _____ (either based on time or number of uses), permitted IP addresses,
	</summary>
		expiration
</details>

<details>
	<summary>
		Amazon's Global Content Delivery Network offering is called _____
	</summary>
		CloudFront
</details>

<details>
	<summary>
		Use signed URLs to restrict access to individual files, or for when your users can't use cookies. Use signed _____ to provide access to multiple restricted files and to avoid having to change your current URLs.
	</summary>
		cookies
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The _____ returns the file if it's present in its cache. Otherwise, the _____ compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the _____ forwards the files to the user and caches them for later.
	</summary>
		POP
</details>

<details>
	<summary>
		Does Cloudfront allow you to specify an origin based on the kind of device accessing it? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Use signed _____ to restrict access to individual files, or for when your users can't use cookies. Use signed cookies to provide access to multiple restricted files and to avoid having to change your current URLs.
	</summary>
		URLs
</details>

<details>
	<summary>
		Can an S3 Bucket be a CloudFront origin? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		CloudFront edge locations can be both _____ and read from.
	</summary>
		written to
</details>

<details>
	<summary>
		Are CloudFront template names unique within your entire AWS account? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in _____ relative to the user. The POP returns the file if it's present in its cache. Otherwise, the POP compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the POP forwards the files to the user and caches them for later.
	</summary>
		latency
</details>

<details>
	<summary>
		CloudFront edge location caches are updated when _____
	</summary>
		something is requested
</details>

<details>
	<summary>
		"You upload files to a CloudFront edge location and have it sync back to the origin by allowing PUT/POST in ""_____"""
	</summary>
		Allowed HTTP Methods
</details>

<details>
	<summary>
		Can a personal webserver be used as an origin server in CloudFront? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to the CloudFront POP (edge location) lowest in latency relative to the user. The _____ returns the file if it's present in its cache. Otherwise, the _____ compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the _____ forwards the files to the user and caches them for later.
	</summary>
		POP
</details>

<details>
	<summary>
		CloudFront edge locations can be both written to and _____.
	</summary>
		read from
</details>

<details>
	<summary>
		An S3 bucket used as a failover page must have its name match the page's domain name. With AWS CloudFront you can configure multiple alternate domain names on the _____.
	</summary>
		distribution
</details>

<details>
	<summary>
		_____ URLs can be created to access objects on CloudFront edge locations. Policies can specify its expiration (either based on time or number of uses), permitted IP addresses,
	</summary>
		Signed
</details>

<details>
	<summary>
		To serve content stored in S3, but not directly accessible from S3, you could create a CloudFront _____ with access to the S3 bucket objects.
	</summary>
		Origin Access Identity (OAI)
</details>

<details>
	<summary>
		Can it be cheaper and faster to deliver content via CloudFront than directly from S3? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Override S3 bucket permissions in CloudFront by using an origin _____.
	</summary>
		access identity
</details>

<details>
	<summary>
		A CloudFront Distribution is a collection of _____
	</summary>
		edge locations
</details>

<details>
	<summary>
		To maximise performance of an image-sharing website so that users can download frequently accessed images quickly from anywhere in the world, you could use AWS _____
	</summary>
		CloudFront
</details>

<details>
	<summary>
		An S3 bucket used as a failover page must have its name match the page's domain name. With AWS CloudFront you can configure multiple _____ on the distribution.
	</summary>
		alternate domain names
</details>

<details>
	<summary>
		A CloudFront _____ is a collection of  edge locations
	</summary>
		Distribution
</details>

<details>
	<summary>
		A user accesses your CloudFront-powered website and requests a file. DNS routes the request to _____ lowest in latency relative to the user. The POP returns the file if it's present in its cache. Otherwise, the POP compares the request with the specifications in your Distribution and downloads the missing file from the origin server. Once the first byte arrives from the origin, the POP forwards the files to the user and caches them for later.
	</summary>
		the CloudFront POP (edge location)
</details>

