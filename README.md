# Lambda-CF-SG-IPs
Lambda function to auto update your security group IP's to allow only CloudFront Global and Regional IPs

## Personal changes to the AWS provided Blog
- [AWS Lambda Cloudfront Blog](https://aws.amazon.com/blogs/security/how-to-automatically-update-your-security-groups-for-amazon-cloudfront-and-aws-waf-by-using-aws-lambda/)

## Reason for changes
I found that having the search use Filters instead of Security Group IDs didn't make much sense to me, I also couldn't get it to work with the Filers.
So instead I decided to modify it to use Security Group IDs.

In order to do this I created two lists, one for the Regional IPs and one for Global
- [CloudFront IP Ranges](https://ip-ranges.amazonaws.com/ip-ranges.json)

The steps to set this up can be found in the [AWS Lambda CloudFront Blog](https://aws.amazon.com/blogs/security/how-to-automatically-update-your-security-groups-for-amazon-cloudfront-and-aws-waf-by-using-aws-lambda/) above.

## LICENSE
[Apache License](./LICENSE)