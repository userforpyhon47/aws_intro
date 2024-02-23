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

- On demand: Se mide en tiempo normalmente de hr/min,/seg
- Reserved: Se reserva instancia de 1 a 3 años. El costo es más barato.
- Spot: Idle computing resource, cheaper but if required AWS can take it back and pause your work. Once done it resumes your process. Not ideal for key job

Riesgos de costos:

- Misconfiguration: Wrongly selecting the size of the services. It is preferred to use architecture templates to have standardized services
- Violación de datos/servicios: Vulnerabilidad dado el resultado de error humano o dado como malas prácticas. E
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
- AWS: Responsability for secuirty of the coud: Infraestructure and sofware that manages that infraestructure

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

- General purpose: 
- Processing optimized
- Memory optimized (rendering processes)
- Accelerated Computing (scientific commputing)
- Storage Optimized (

Naming convention:

m(family)5(generation).(size)
- Family: m, t, c
- Generation: 1, 2, 3, ...
- Size: large, lx, 2xlarge





