emplate that will create the following:

API Gateway:
Deployed as a REGIONAL endpoint.
Single root method, accepting POST requests only, with Lambda proxy integration to a target function.
In-line Python Lambda function echoing back requesting users IP address to API Gateway requests:
IAM role for Lambda allowing CloudWatch logs access.
Permissions for Lambda that allow API Gateway endpoint to successfully invoke function.
CloudWatch logs group for Lambda, with 90 day log retention.


you will be able to make a HTTP POST request to the URL listed as the apiGatewayInvokeURL output value.

$ curl --request POST https://APIGW_ID.execute-api.AWS_REGION.amazonaws.com/call