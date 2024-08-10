# AWS-Diagrams

mindmap
  root((AWS Cloud Practitioner Certification))
    Concepts
      Security
        IAM
          Definition: Identity and Access Management
          Key: Manage users, groups, roles, policies
          Limitation: Region-specific, initial setup complexity
        Shared Responsibility Model
          Definition: Security responsibilities between AWS and the customer
          Key: AWS manages infrastructure, customer manages data and applications
          Common: Clear division of responsibilities
        Compliance
          Definition: AWS compliance programs and certifications
          Key: GDPR, HIPAA, SOC, PCI DSS
          Limitation: Customer still responsible for compliance
        Security Groups
          Definition: Virtual firewall for instances
          Key: Control inbound and outbound traffic
          Limitation: Limited to VPC
      Cloud Concepts
        Regions and Availability Zones
          Definition: Geographic locations and isolated zones
          Key: High availability, fault tolerance
          Limitation: Latency between regions, service availability
        VPC
          Definition: Virtual Private Cloud
          Key: Isolated network, subnets, route tables, gateways
          Limitation: VPC peering limits, CIDR block limits
        Elastic Load Balancing
          Definition: Distributes incoming traffic across targets
          Key: High availability, fault tolerance, scaling
          Limitation: Limited to certain instance types
        Auto Scaling
          Definition: Automatically adjusts capacity
          Key: Maintain performance, cost-efficiency
          Limitation: Scaling limits, configuration complexity
      Pricing and Billing
        Free Tier
          Definition: Limited free usage of AWS services
          Key: Test and learn AWS
          Common: 12-months free for new customers, always free services
          Limitation: Limited usage per service
        Cost Management
          Definition: Tools for tracking and managing costs
          Key: Budgets, cost explorer, cost allocation tags
          Common: Alerts for budget thresholds
        Billing and Pricing Tools
          Definition: Services to monitor and control spending
          Key: AWS Pricing Calculator, Billing Dashboard
          Common: Pay-as-you-go pricing
        TCO Calculator
          Definition: Total Cost of Ownership Calculator
          Key: Compare on-premises and AWS costs
          Common: Cost comparison, migration planning
        Saving Plans
          Definition: Commit to usage for reduced cost
          Key: Flexible pricing, long-term savings
          Limitation: Commitment required, specific service plans
      Support
        AWS Support Plans
          Definition: Different levels of support
          Key: Basic, Developer, Business, Enterprise
          Common: Varying levels of support access and response times
        Documentation
          Definition: AWS resource and service documentation
          Key: User guides, API references, tutorials
          Common: Comprehensive, regularly updated
    Core Services
      Compute
        EC2
          Definition: Elastic Compute Cloud
          Key: Scalable virtual servers
          Limitation: Instance limits, region availability
        Lambda
          Definition: Serverless compute service
          Key: Run code without provisioning servers
          Limitation: Execution duration limits, memory limits
        Elastic Beanstalk
          Definition: Platform as a service
          Key: Deploy and manage applications
          Limitation: Limited customization
        ECS
          Definition: Elastic Container Service
          Key: Run and manage Docker containers
          Limitation: Cluster capacity limits
      Storage
        S3
          Definition: Simple Storage Service
          Key: Scalable object storage
          Limitation: Object size limits, request rate limits
        EBS
          Definition: Elastic Block Store
          Key: Block storage for EC2
          Limitation: Volume size limits, snapshot limits
        Glacier
          Definition: Low-cost archive storage
          Key: Long-term data archiving
          Limitation: Retrieval times, archive size limits
        EFS
          Definition: Elastic File System
          Key: Scalable file storage
          Limitation: Performance mode limits, region availability
      Database
        RDS
          Definition: Relational Database Service
          Key: Managed relational databases
          Limitation: Instance limits, storage limits
        DynamoDB
          Definition: NoSQL database service
          Key: High performance, scalable
          Limitation: Item size limits, request rate limits
        Redshift
          Definition: Data warehousing service
          Key: Analyze data using SQL
          Limitation: Node limits, query limits
        Aurora
          Definition: MySQL and PostgreSQL compatible
          Key: High performance managed database
          Limitation: Instance limits, region availability
    Management and Governance
      CloudWatch
        Definition: Monitoring and observability service
        Key: Metrics, logs, alarms
        Limitation: Retention limits, metric limits
      CloudTrail
        Definition: Logging and monitoring API calls
        Key: Governance, compliance, auditing
        Limitation: Event history limits, region limits
      CloudFormation
        Definition: Infrastructure as code
        Key: Create and manage resources with templates
        Limitation: Stack limits, template size limits
      AWS Config
        Definition: Resource configuration management
        Key: Continuous monitoring, compliance auditing
        Limitation: Configuration recorder limits, rule limits
    Networking and Content Delivery
      VPC
        Definition: Virtual Private Cloud
        Key: Isolated network, security controls
        Limitation: VPC peering limits, CIDR block limits
      Route 53
        Definition: Domain Name System (DNS) service
        Key: Domain registration, routing, health checks
        Limitation: Query limits, domain limits
      CloudFront
        Definition: Content Delivery Network (CDN)
        Key: Low latency, high transfer speeds
        Limitation: Cache invalidation limits, region availability
      API Gateway
        Definition: Create and manage APIs
        Key: Secure, scalable APIs
        Limitation: Request limits, integration limits
    Analytics
      Athena
        Definition: Serverless interactive query service
        Key: Analyze data in S3 using SQL
        Limitation: Query limits, data source limits
      QuickSight
        Definition: Business intelligence service
        Key: Visualize data, create dashboards
        Limitation: User limits, data source limits
      Glue
        Definition: ETL (Extract, Transform, Load) service
        Key: Data preparation and integration
        Limitation: Job limits, data catalog limits
      Kinesis
        Definition: Real-time data processing
        Key: Stream data analytics
        Limitation: Shard limits, data retention limits
    Developer Tools
      CodeCommit
        Definition: Source control service
        Key: Managed Git repositories
        Limitation: Repository limits, file size limits
      CodeBuild
        Definition: Build and test code
        Key: Continuous integration
        Limitation: Build duration limits, concurrent build limits
      CodeDeploy
        Definition: Automate code deployments
        Key: Consistent deployments
        Limitation: Deployment limits, instance limits
      CodePipeline
        Definition: Continuous delivery service
        Key: Automate release pipelines
        Limitation: Pipeline limits, action limits
    Application Integration
      SNS
        Definition: Simple Notification Service
        Key: Publish/subscribe messaging
        Limitation: Topic limits, message size limits
      SQS
        Definition: Simple Queue Service
        Key: Message queuing
        Limitation: Message size limits, queue limits
      SWF
        Definition: Simple Workflow Service
        Key: Coordinate distributed applications
        Limitation: Task execution limits, workflow limits
      Step Functions
        Definition: Coordinate multiple AWS services
        Key: Build and run workflows
        Limitation: State machine limits, execution limits
    Machine Learning
      SageMaker
        Definition: Build, train, deploy ML models
        Key: Fully managed ML service
        Limitation: Instance limits, model size limits
      Rekognition
        Definition: Image and video analysis
        Key: Object detection, facial recognition
        Limitation: Image size limits, request rate limits
      Lex
        Definition: Build conversational interfaces
        Key: Chatbots
        Limitation: Intent limits, request limits
      Comprehend
        Definition: Natural Language Processing (NLP)
        Key: Text analysis, sentiment analysis
        Limitation: Document size limits, request rate limits


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
