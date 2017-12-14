# Architecture principles
Architecture principles are descriptive (not prescriptive) patterns emerging from good design. The intention of having architecture principles is to conclude on common guardrails that allow us to drive faster and feel more safe when making decisions.

Our architectural approach is not to strictly follow principles as rules but rather make them visible by good work of IT architecture community.​​​

![](/assets/guardrails.png)

The list below is not an all-encompassing list of best practices, but a set of key principles we want to focus on in 2018

# General
## G1 – Re-use before Buy before Build
> **By** investigation of the existing landscape for matching platforms and solutions to be re-used, before market investigation for packaged solutions and configuration rather than customisation of these solutions, before building via bespoke development, **it is ensured that** the technology diversity of the IT landscape is reduced **so that​** IT cost and complexity is minimised.

### Implications
* IT solutions are designed with an emphasis on future re-use
* Created components of IT solutions are registered in the architecture repository and can be easily and quickly found
* Creation of reusable solutions typically requires higher initial costs

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>​Processes, data, applications, technologies and other IT components are used in multiple business contexts</li><li>The implementation time of projects is decreasing due to re-using of available components</li><li>Commodity procedures (like customer identity management, etc.) are unified for all solutions</li></ul> | <ul><li>​​The same or similar functionalities are implemented multiple times within the IT landscape</li><li>IT solutions are designed from scratch and are competing with standard available products on the market</li><li>Infrastructure is established for each purpose independently and is not shared</li></ul>

### Further reading
* TBD

## G2 – Maximize company benefits
> **By** considering benefits of every solution design in the light of whole company rather than evaluating it only from isolated perspective **it is ensured that** architectural changes creates the highest long-term value for the company **so that** no locally beneficial approach might make negative impact on overall business landscape.

### Implications
* All decisions and solution designs are assessed towards whole company benefits
* Positive benefit for whole company might have negative impact to its isolated part
* Implementation of solutions with maximized benefits for the company might be more expensive than implementation locally oriented designs

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Locally implemented solutions are beneficial for the whole company (or at least does not have negative impact to whole company)</li><li>Implemented solutions create value for whole company therefore they are re-usable within the company regardless the place of origin</li><li>Considerations of whole company benefits are obvious part of architecture decision making procedures</li></ul> | <ul><li>Locally implemented solutions does not create value for the whole company (or even worse make negative impact from the whole company perspective)</li><li>Company wide benefits considerations are not part of architecture decision making procedures</li></ul> |

### Further reading
* [THINK ENTERPRISE FIRST](http://www.biske.com/blog/?p=878)

## G3 – Commit to common EAM approach
> **By** building common Enterprise Architecture capability and working as company wide IT architecture community **it is ensured that** the cross-segment relevant transparency is established to support capability and information share and individual IT segments are not isolated in their silos **so that** the synergies are easily identified and architectural re-use is enabled across segments.

### Implications
* Ownership of EAM is not with a central team, but the different architects define a common minimum data model and use a central tool to consolidate information
* The central tool is integrated into our processes – EAM is successful when the information is actively used within our processes (CMDB, Billing, Service Management, …)
* Segment IT can adopt the central tool (Renewables, Corporate, potentially Retail) or continue to use existing tools (ARIS in case of Grid) if they desire, as long as an automated integration to the central tool is in place

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Segment architects together with central EA team contributes together to create common EA capability</li><li>Agreed level of transparency about IT assets in segment IT is achieved for cross-segment purposes</li><li>IT processes benefit out of the available information from all segments IT (impact analysis, lifecycle management, etc.)</li></ul> | <ul><li>​​Different levels of transparency about IT assets exist in individual segments</li><li>​​​​Sharing capabilities and information is complicated due to fragmented information silos and lingos</li><li>Synergies are achieved by coincidence​</li></ul> |

### Further reading
* TBD

# Applications and Integration

## A1 – Mesh App & Service architecture (MASA)
> **By** creating cloud-native, web-scale, modular and adaptive solutions that can be continuously and rapidly modified and refactored **it is ensured that** services are encapsulated and exposes APIs at multiple levels and across organizational boundaries, balancing the demand for agility and scalability of services with composition and reuse of services **so that** designed solutions provide a solid foundation for digital business ecosystems.

### Implications
* 
* 
* 

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li></li><li></li><li></li></ul> | <ul><li></li><li></li><li></li></ul> |

### Further reading
* TBD

## A2 – Leverage on platforms
> **By** designing IT solutions based upon platforms (at all levels of IT landscape) rather than developing everything from scratch **it is ensured that** the implemented logic is separated from the technical solution **so that** the impact of technical changes to business processes and vice-versa is reduced.

### Implications
* Investigation of available platforms has to be an inevitable part of IT solution design - even across particular IT segments
* As leverage platforms is innogy IT strategy, using platforms expects trust among teams and assumes advocacy of platforms usage beyond IT discussions
* Platforms built with the intention of re-use has to be properly documented in shared environment so that it is easy to find such platforms while working on design of IT solutions

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Technical changes are not the issue while changing the business logic of IT solutions​</li><li>Common capabilites are quickly accessible, ready to use, secure, scalable and tested</li><li>Solutions are developed by assembly of Platform services from one or more platforms, augmented with solution specific capabilities</li></ul> | <ul><li>Every IT solution is like a snowflake - no unified approach to commodity IT exists</li><li>Productivity of DevOps teams is limited by having to deal with maintenance of their own tools</li><li>Effectivity of IT delivery is wasted on repetitive building of commodity IT</li></ul>

### Further reading
* TBD

## A3 – Think Cloud-Native \(Cloud-First\)
> **​By** developing cloud-native applications based on 12-factor methodology **it is ensured that** maximum agilitiy is achieved by continuous deployment and minimized divergence between development and production, **so that** the apps can be scaled up and down without significant changes to tooling, architecture, or development practices.

### Implications
* Organizational and cultural aspects have to be considered by development teams to follow the self-service and DevOps approach
* In case of external development or buying of development from the market, it has to be ensured that the 12-factor methodology is applied
* Agile and DevOps might be tricky to be accepted by some parts of the organization but it does not provide any reason to stop advocating this principle​

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Applications offer maximal portability among execution environments</li><li>Software delivery pipelines are automated end-to-end due to increased collaboration between development and IT operations team with a shared responsibility.</li><li>Architecture of the applications is based on microservices (smaller independently deployed applications integrated together to achieve ​robustness)</li></ul> | <ul><li>Cloud computing delivery model does not bring expected benefits as its usage stays on the level of another infrastructure provider</li><li>Applications are heavily depending on underlying infrastructure (the infrastructure is not transparent)</li><li>Company will not be competitive in digital markets due to high time to market caused by low autonomy of application developers and application architecture working against agility</li></ul>

### Further reading
* [The Twelve-Factor App](https://www.12factor.net/)

## A4 – Loosely coupling to mitigate constraints
> **By** designing IT components that could be used without the knowledge of internal implementation and integrating them the way that changes of interfaces do not make impact to the existing integrations **it is ensured that** the IT landscape is robust to changes **so that** the integration costs decrease and the quality and stability of IT environment increase in time.

### Implications
* All IT components are integrated through some integration layer (e.g. message queues) that reduce the dependency of IT components on each other
* Implementation costs of projects and changes might temporarily increase until the benefits of decreased dependencies will outreach
* Data transfered by interfaces should be published in open standard formats (e.g. XML, JSON, etc.)​

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Changes of IT integration interfaces does not break the IT landscape</li><li>IT components are easily replaceable by alternative implementations providing the same services</li><li>IT maintenance complexity decrease due to independency of IT components within the IT landscape</li></ul> | <ul><li>Every change in IT integration interface must be reflected to all interface consumers so their contracts are not breached</li><li>Complexity of IT landscape changes increase with the increasing number of integrations</li><li>​​IT components are depending on underlying infrastructure and also cannot be easily replaced by alternative implementations due to high complexity and dependencies​</li></ul> |

### Further reading
* TBD

# Data and Information

## D1 – Share before replicate
> **By** preferring managed access to existing master sources of data by functional services rather than replicating unmanaged number of the same data within the landscape **it is ensured that** the overall data quality and value increase **so that** the data governance is simplified and the data are catalogued for future re-use.

### Implications
* Managing data in unified data sources allows to keep the desired data quality and minimize wrong data usage and interpretation
* Data are exposed as functionally oriented services so other applications does not consume the data for further processing but performing the functions and present the results further
* Services and their data are cataloged for easier retrieval and reuse.

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>The data is managed in defined (and unified) sources and are processed by execution of functionally oriented services</li><li>The data is not replicated between systems (if not required)</li><li>The data sources are known and documented including the data owners</li></ul> | <ul><li>The data is replicated between applications to achieve loosely coupling and reduce applications interdependence.</li><li>Services are data and not functionally oriented.</li><li>Services are used as data pumps that provide data that is then arbitrarily processed by a consumer of the service.</li></ul> |

### Further reading
* TBD

## D2 – Secure company data
> **By** approaching data as an company digital asset, applying conscious data access management, relevant encryption and not leaving any data unprotected **it is ensured that** every piece of data is accessible only to authorized people and data protection is inevitable part of every data-related decision **so that** the risks of data misuse, data leaks or thefts are mitigated.

### Implications
* Data is classified according to its security requirements and limited work is part of company regulations.
* Data is secured in its repository during processing and protected from unauthorized access.
* Data in non-production environments is malformed or masked so that it can not be misused.

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li></li><li></li><li></li></ul> | <ul><li></li><li></li><li></li></ul> |

### Further reading
* TBD

# Technology

## T1 – Promote API-led integration
> **By** enabling the integration APIs to be reused by many parties and also inside the integration platforms and by organizing APIs to layers (System, Process and Experience) **it is ensured that** the developers evolve the business logic faster and safer way (less bugs due to re-use already tested APIs) **so that** whole IT becomes a big platform to support business digital transformation.

### Implications
* 
* 
* 

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li></li><li></li><li></li></ul> | <ul><li></li><li></li><li></li></ul> |

### Further reading
* TBD

## T2 – Avoid technical lock-in
> **By** designing IT solutions the way that the desired function does not depend on specific technology or vendor **it is ensured that** all components of the design or vendors could be replaced without significant effort or re-design of the solution **so that** the most effort can be spent on the business outcomes and not on the technical issues and the dependency on particular technologies is minimal.

### Implications
* 
* 
* 

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li></li><li></li><li></li></ul> | <ul><li></li><li></li><li></li></ul> |

### Further reading
* TBD

## T3 – Follow open standards
> **By** preferring of verified open standards within designed solutions before closed or proprietary stuff **it is ensured that** the implementation, documentation, training and maintenance efforts are significantly reduced and designed solutions and integrations are easier understandable to new team members and also to partners **so that** IT development and operations costs are decreased and the productivity is boosted.

### Implications
* 
* 
* 

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li></li><li></li><li></li></ul> | <ul><li></li><li></li><li></li></ul> |

### Further reading
* TBD