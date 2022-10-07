## Enable CI/CD of multi-Region Amazon SageMaker endpoints

Amazon SageMaker and SageMaker inference endpoints provide a capability of training and deploying your AI and machine learning (ML) workloads. With inference endpoints, you can deploy your models for real-time or batch inference. The endpoints support various types of ML models hosted using AWS Deep Learning Containers or your own containers with custom AI/ML algorithms. When you launch SageMaker inference endpoints with multiple instances, SageMaker distributes the instances across multiple Availability Zones (in a single Region) for high availability. 

In some cases, however, to ensure lowest possible latency for customers in diverse geographical areas, you may require deploying inference endpoints in multiple Regions. Multi-Regional deployment of SageMaker endpoints and other related application and infrastructure components can also be part of a disaster recovery strategy for your mission-critical workloads aimed at mitigating the risk of a Regional failure. 

SageMaker Projects implements a set of pre-built MLOps templates that can help manage endpoint deployments. In this post, we show how you can extend an MLOps SageMaker Projects pipeline to enable multi-Regional deployment of your AI/ML inference endpoints.


## Solution Overview

SageMaker Projects deploys both training and deployment MLOPs pipelines; you can use these to train a model and deploy it using an inference endpoint. To reduce complexity and cost of a multi-Region solution, we assume that you train the model in a single Region and deploy inference endpoints in two or more Regions.

Please refer to this [blog](https://aws-blogs-prod.amazon.com/machine-learning/?p=43952) for step-by-step walkthrough of a solution that slightly modifies a SageMaker project template to support multi-Region deployment.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

