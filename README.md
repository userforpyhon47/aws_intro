# aws_intro
This is notebook for the course of AWS solutions architect

### Day 1.
- Inició con solo 3 servicios: cómputo, almacenamiento y gestión de usuarios

### Principle 5-3-2

(5) Five characteristics of cloud
  - On demand self service: Any service can be provided by the a common user
  - Ubiquitous network access: Accesible via the internet
  - Location transparent resource pooling: 
  - Rapid elasticity: Ability to increase vertically or horizontally the resources
  - Measure service with per use:

(3) Three delivery methods:
  - SaaS: Fully flegde application. Mainly subscription based
  - PaaS: Provide developers to quickly develope applications and focus on features rather than provision and maitaing infra
  - IaaS: You manage underlying compute instances

(2) Two implementation models:
  - Public Cloud
  - Private Cloud

### Day 2. 

Target to review AZ and core services

Costos en la nube:

- On demand: Se mide en tiempo normalmente de hr/min/seg
- Reserved: Se reserva instancia de 1 a 3 años. El costo es más barato.
- Spot: Idle computing resource, cheaper but if required AWS can take it back and pause your work. Once done it resumes your process. Not ideal for key job

Riesgos de costos:

- Misconfiguration: Wrongly selecting the size of the services. It is preferred to use architecture templates to have standardized services
- Violación de datos/servicios: Vulnerabilidad dado el resultado de error humano o dado como malas prácticas.
- Failure in the services:
- Data loss: 
- Account theft: If someone hack your computers

On-premise architecture.
- Location: In house resource
- Management: Specialized personnel to manage storage, network, security and so on
- Scalability: Limited resources cannot grow on demand
- Costs: High upfront cost to purchase all the IT architecture.
- Security: Client has the total control of the security of its resources
- Conectivity: 

Cloud architecture.
- Location: A provider's data center
- Management: Physical management of infraestructure does not belong to the costumer
- Scalability: Scale on demand
- Costs: Pay as you use.
- Security: Physical security
- Conectivity: End costumer needs to have an internet connection

Shared reponsability model:
- Customer: Responsibility for security in the cloud, apps, data
- AWS: Responsability for security of the coud: Infraestructure and sofware that manages that infraestructure

Availability zones:

These are a discrete set of datacenters located in different regions and countries. Currently they have 105 AZ

- A AZ can have up to 6 discrete datacenter
- Independent of each other
- Conection between AZ using dedicated high speed lines
- AWS recomends to do inter AZ replication

Edge location: A delivery point of content. Normally for CDN. Some services located to work in this edge locations:

- CloudFront
- Route53
- AWS Firewall Manager

EC2: Elastic Cloud Computing (virtual machine)
- To create a new instace, it uses AMI (Amazon Machine Image) which is a VM configurable VM template to allow VMs to be launched rapidly
- EC2 needs EBS to be attached

Type of EC2

- General purpose
- Processing optimized
- Memory optimized (rendering processes)
- Accelerated Computing (scientific commputing)
- Storage Optimized

Intances naming convention:

m(family)5(generation).(size)
- Family: m, t, c
- Generation: 1, 2, 3, ...
- Size: large, lx, 2xlarge

## 4. Sesión 4

### 4.1 Review of instaces types:

- General Purpose: Balances compute, memory and networking resources. Great for a wide range of workloads
- Computing Optimized: Offers high performance processors. Ideal for cumpute intensive and batch processing applications
- Memory Optimized: Deliver fast performance memory intensive workloads. Well suited or high performance databases
- Acceletared computing: Uses hardware accelerators to expedited data processing. Ideal for application streaming and graphics workloads
- Storage Optimized: Suitable for workloads such as distributed file system and data warehousing applicatioms

Review of instances cost:

- On-demand: No upfront cost or contract. Ideal for short period lifetime or irregular workloads
- Spot: Offers saving over on demand instances. Ideal for workloads with flexibe start and endtime
- Reseved: Provides a billing discount over on demand pricing. Requires 1 year or 3 year contract commitment
- Compute saving: Offers up to 72% saving over on-demand cost for a consitent amount of compute usage. Requires 1 year o 3 year contract commitment
- Dedicated Instance: An EC2 instance that runs in a VPC on hardware for a sigle customer.
- Dedicated host: A physical server with EC2 instance for a single customer

### 4.1 Autoscaling and Load Balancing

- Autoscaling:
Scale capacity as computing requirements change using dynamic and predictive horizontal scaling.

What is an auto-scaling group? An object that defines the minimun and maximun number of instances a group is allowed to have based on scaling computing requirements. 

- Load balancing:
Automatically distributes traffic across distributed resources providing a single point of contact. Usually it is recommended to attach a load balancing to a auto scaling group.

### 4.2 AWS Messaging services

Newer application arquitectures are based on microservices decoupling services and providing standard integration interfaces for inter service communication.

- SNS: Simple Notification Service
Notifications as published into topics. Subscribers of the topic will receive the notification

### 4.3 Serveles Compute Services

No need to create and manage the underlying infrastructure to run code.

AWS Lambda: Code that is executed after an event is triggered in AWS without the need to manage a EC2 instance. Not suitable for computing tasks that consume a computing time more than 15 mins.

### 4.4 AWS Container Services


