# gameplay-analytics-pipeline
The gameplay-analytics-pipeline is a serverless analytics pipeline that provides a solution for ingesting telemetry events from games and backend services. This application has been extended from the [Implementation Guide](https://docs.aws.amazon.com/solutions/latest/game-analytics-pipeline/welcome.html) from AWS and includes additional features such as a user-interface for accessing the solution API and a build/release pipeline. Changes are made incrementally and can be accesed via the release notes section of this repository. 

## Build/Release Pipeline
The build/release pipeline is a multi-account, enterprise-grade, dynamic branch pipeline for the serverless analytics pipeline application. The build/release pipeline has been extended from the [Implementation Guide](https://aws.amazon.com/solutions/partners/serverless-cicd-for-enterprise/) from AWS partner solution Trek10.
  
The build/release pipeline uses several AWS services to enable multiple development teams within an organization to collaborate on serverless application deployments. The following AWS resources are provisioned:

* AWS Identity and Access Management (IAM) users, roles, and groups in your AWS development, production, and shared services accounts to control access to pipeline actions and deployed resources.
* Dynamic branch pipelines for deploying and testing new feature code in Git branches, using AWS CodePipeline.
* A master code pipeline that deploys to multiple AWS accounts, using AWS CodePipeline.
* An AWS CodeCommit repository for storing application code.
* Amazon Simple Storage Service (Amazon S3) buckets for pipeline artifacts.
* AWS Secrets Manager to store sensitive configuration data in a central location.
* AWS CodeBuild and AWS CodeDeploy configurations for building, deploying, and testing serverless applications.
* A sample serverless application that uses AWS Lambda, Amazon API Gateway, and Amazon DynamoDB.
* Integration with other Amazon services such as AWS Lambda, AWS Key Management Service (AWS KMS), and Amazon Simple Notification Service (Amazon SNS).