# Serverless

## What is serverless?
```
"Serverless is the native architecture of the cloud that enables you to shift more of your operational responsibilities to AWS, increasing your agility and innovation. Serverless allows you to build and run applications and services without thinking about servers. It eliminates infrastructure management tasks such as server or cluster provisioning, patching, operating system maintenance, and capacity provisioning. You can build them for nearly any type of application or backend service, and everything required to run and scale your application with high availability is handled for you." - aws.amazon.com
```

## Why to use serverless?
```
"Serverless enables you to build modern applications with increased agility and lower total cost of ownership. Building serverless applications means that your developers can focus on their core product instead of worrying about managing and operating servers or runtimes, either in the cloud or on-premises. This reduced overhead lets developers reclaim time and energy that can be spent on developing great products which scale and that are reliable." - aws.amazon.com
```

There are bunch of serverless services that are available from different cloud servide providers. Here I am going to explain some of AWS serverless servceis.

###  Computing Serverless Services
AWS provides different computing serverless services such as AWS Lambda, Lambda@Edge and AWS Fargate. Lambda is the FaaS implementation on AWS cloud. It supports different language runtime and provides FaaS services. There are different versions computing serverless services on AWS such as, .

### Storage Serverless Services
AWS has two different storage serverless services which are Amazon S3 and Amazon EFS. 
Amazon S3 provides object storage service that has the feature of easily scalable. Applications that use AWS Lambda, stores their files using Amazon S3, for example, S3 is used to store or archive the data for website, mobile application, enterprise applications, IoT devices, and big data. The basic storage units of S3 are objects which are organized into buckets. 
Amazon S3 can be used to replace significant existing static web-hosting infrastructure with HTTP client accessible objects. The AWS authentication mechanism allows the bucket owner to create an authenticated URL which is valid for specific amount of time.
![](https://geekylane.com/wp-content/uploads/2019/05/Static-Website-Using-S3-Bucket-.png)

### Data Stores Serverless Services
