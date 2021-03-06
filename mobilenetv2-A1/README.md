Deploy Mobilenet_v2 on AWS
------------------------------------------------------------------------------------------------------------
----------------------
## Notes 
---------------------------------------------------------------------------------------------------------------------------

1) Deployed pretrained mobilenet_v2 on AWS Lambda. Predicted the class id and class name for the [Yellow Labrador Retriever](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/Yellow-Labrador-Retriever.jpg) image. 
This is our [API Gateway URL](https://om2aap1ekh.execute-api.ap-south-1.amazonaws.com/dev/classify)

![insomnia](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/Insomnia%20request-response.png)

2) Used [imagenet-simple-labels.json](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/src/imagenet-simple-labels.json) file to retrieve the labels for the imagenet class id's.
Got the imagenet labels in json format from this github repo [imagenet-labels](https://github.com/anishathalye/imagenet-simple-labels)


2) Downloaded pretrained mobilenet_v2 model using [mobilenet_v2.py](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/src/mobilenet_v2.py)

3) Uploaded mobilenet_v2.pt to AWS S3 bucket. 

![s3_bucket](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/S3%20bucket.JPG)

4) Followed steps mentioned in the session and uploaded a docker package (container) [mobilenetv2-a1.zip](https://mobilenetv2-a1-dev-serverlessdeploymentbucket-1nd2vtd912kbg.s3.ap-south-1.amazonaws.com/serverless/mobilenetv2-a1/dev/1594790813774-2020-07-15T05%3A26%3A53.774Z/mobilenetv2-a1.zip) to AWS.

---------------------------------------------------------------------------------------------------------------------------
## Prediction for different classes present in imagenet dataset

<img src="https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/hummingbird.png" width="80%" height="80%">

<img src="https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/spaceshuttle.png" width="80%" height="80%">

---------------------------------------------------------------------------------------------------------------------------
## Cloudwatch Logs

![cloudwatchlogs](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/AWS%20cloudwatch%20request%20log.png)

---------------------------------------------------------------------------------------------------------------------------
## API Gateway details

![apigatewaydetails](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/AWS%20API%20gateway%20details.png)

---------------------------------------------------------------------------------------------------------------------------
## API Gateway Dashboard

![apigatewaydashboard](https://github.com/csharpshooter/E4P2/blob/master/mobilenetv2-A1/images/AWS%20API%20gateway%20dashboard.png)
