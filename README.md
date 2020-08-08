# FaaS-Study
Cloud service providers offer their services in form of as-a-service such as:
- Infrastructure as a Service (IaaS)
- Platform as a Service (PaaS)
- Container as a Service (CaaS)
- Backend as a Service (BaaS)
- Function as a Service (FaaS)
- Software as a Service (SaaS)

Each of these services have different level of abstraction to access the underlying resource network. Infrastructure as a Service (IaaS) offer a very low-level service and put all the burden of managing virtual machine to users and most of the cases, users don't want to have this responsiblity of managing servers, instead they want to focus on development of code. Here comes the FaaS use cases where it makes the DevOps to NoOps and remove the burden of managing server from users, instead users can only focus on the development of code. 
Through FaaS, you can run your application by uploading the zip of source code to the FaaS platform and everything else will be managed by FaaS provider or FaaS platform. Let's say, we want to develop an application for a new start up company, instead of choosing other services, FaaS is a an excellent choice to make new start up application happen faster and less cost of running the application. Yes, FaaS costs less compare to other platforms because you pay as per function call, instead of paying for running the entire server. 

Almost all the public cloud services provide FaaS, such as AWS Labmda, Google Cloud Functions, Azure Functions, etc. Even open source FaaS platforms are available such as OpenFaaS, OpenWhisk, Serverless, etc. The trend to using FaaS is increasing and majority of the companies which are using cloud services are tending to migration to FaaS due to FaaS's unique features.

Some of the characteristics of FaaS are:
- Pay-as-you-go (pay per 100 milliseconds)
- Easily scale out of functions (concurrency)
- Triggered based running
- Easily-integrated
- Stateless

When we talk about Serverless, FaaS is an example of Serverless, where there are many types of serverless serivces such as Amazon Simple Storage Service (Amazon S3), Amazon Elastic File System (Amazon EFS), Amazon DynamoDB, Amazoin Aurora Serverless, Amazon RDS Proxy, Amazon API Gateway, Amazon SNS, Amazon SQS, Amazon AppSync, Amazon EventBridge, Amazon Kinesis, Amazon Athena, etc. Each of these services are an example of Serverless and FaaS the the most famous implementation of FaaS. Each of these services will be used by FaaS as glue component in the middle.

![](https://blogs.itemis.com/hs-fs/hubfs/Blog%20(2019)/Software%20Development/Creating%20serverless%20applications%20on%20AWS/Serverless%20data%20pipeline.png?width=1024&name=Serverless%20data%20pipeline.png)

Different cloud providers support different language runtime enviornments, such as AWS lambda support `NodeJs`, `Python`, `Java`, `Go`, `C#`, and custom runtime. It differs from one cloud provider to next in terms of language support, but almost all of them support the NodeJS and python by default. This indicates that majority of applications running on FaaS are writtin in Python and NodeJS.

Beside all the advantages FaaS brings, it has many challenges too which comes to the cost of having good features. The first challenge FaaS faces is platform-overheads or its called cold-start time.
Cold start time is the time to create a new function instance on a new container when there's not available the warm container. Since FaaS runs on trigger based mechanism and containers only live for around 5 minutes while being unused, so to not waste teh resources, unsed Function containers are stopped and when there are now available running container for FaaS, new container are created which for sure, creating a new container takes time and the time it takes depend on platform type and its between 50ms and 14 seconds. The second challange FaaS faces is the hardware hetrogeneity that makes the predication of time execution diffult. Since FaaS is connected to different other services and these hetrogenious services makes the FaaS overfall performance dependent on them, therefore, the overall performance of FaaS is depdents on external services as well. The third challange that FaaS faces is the complex triggering mechanism. 


FaaS performance Benchmark
For sure, FaaS as any other cloud services should have some benchmarks, therefore, we have two main benchmarks for FaaS. Micro-benchmark and Application benchmarks. 
The micro-benchmark focuses on low-level performance of FaaS platforms such as CPU, Network and I/O, but mainly used for CPU performance, and application-benchmark is used to calculate the overall performance of a FaaS application. 
There are available workload tests to evaluate each benchmark, such as [FaaSBench](https://github.com/kmu-bigdata/serverless-faas-workbench) which provides workload tests for different cloud providers such as AWS Lambda, Google Cloud Function, and Azure Functions. FaaSBench has workloads for testing the performance of FaaS Network, I/O, and CPU performance as well as it has workload tests for application benchmarks too. 
