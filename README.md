# AWS KMS encryption example

This example show how AWS KMS key should be used for encoding values, that can be then decoded in AWS Lambda


To run this code you should path AWS KMS key arn as Program parameter.

arn key pattern is next - "arn:aws:kms:us-west-2:${uniqueId}:key/${KmsKeyUUID}.

It can be found on key page in AWS console.

Depends on region created.


It will print out encrypted value encoded by Base64 AWS funciton of string "MY SDK ENCRYPTED value"

In Base64 encoded value it should be passed as ENV variables to AWS Lambda