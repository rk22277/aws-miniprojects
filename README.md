# aws-miniprojects
This is an AWS mini project 

Thanks to Adrian Cantrill for all the awesome AWS projects which help in understanding the services better

This is a event driven serverless pixalator application in which an s3 object put triggers a lambda function which generates 5 pixelated images of 8X8, 16X16, 32X32, 48X48, 64X64

Create two S3 Buckets, source and processed

An IAM role is created for lambda to call aws service(s3 here) on your behalf with an inline policy defined

Lambda function is created using a zip file with python file and pillow installed(check for compatability between two), update configurations to add key-value where value would be the processed bucket. Add a trigger for s3 source bucket, where each put event would invoke the lambda function generating 5 pixelated images in processed bucket

The results of the projects can be found in results folder
