# AWS-Diagrams

```mermaid
graph TD
  A[Compute Services]
  A --> B[EC2]
  B --> B1[Scalable virtual servers]
  B --> B2[Full control over instances]
  A --> C[Lambda]
  C --> C1[Serverless compute]
  C --> C2[Event-driven execution]
  A --> D[Elastic Beanstalk]
  D --> D1[Platform as a Service]
  D --> D2[Automatic scaling and monitoring]
  A --> E[ECS]
  E --> E1[Docker container management]
  E --> E2[Integration with EKS and Fargate]
