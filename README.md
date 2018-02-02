# Architecture principles
Architecture principles are descriptive (not prescriptive) patterns emerging from good design. The intention of having architecture principles is to provide common guardrails that allow us to move faster and feel safe when making decisions.

Our architectural approach is not to strictly follow principles as rules but rather make them visible through the good work of the IT architecture community.​​​

![](/assets/guardrails.png)

The list below is not an all-encompassing list of best practices, but a set of key principles we want to focus on in 2018

# General
## G1 – For non-differentiating IT: Re-use before Buy before Build
> **By** investigation of our existing landscape for matching platforms and capabilities to be re-used, before conducting a market investigation for packaged solutions and configuration, before bespoke solution development, **it is ensured that** the technology diversity of our IT landscape is reduced, **so that** IT cost and complexity are minimised for maximum efficiency.

### Implications
* IT solutions are designed with an emphasis on future re-use
* Created components of IT solutions are registered in the architecture repository and can be easily and quickly found
* Creation of reusable solutions typically requires higher initial costs

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>​Platforms, processes, data, applications, technologies and other IT components and services are used in multiple business contexts</li><li>The implementation time of projects is decreasing due to re-using of available components</li><li>Commodity procedures (like customer identity management, etc.) are unified for all solutions</li></ul> | <ul><li>​​The same or similar functionalities are implemented multiple times within the IT landscape</li><li>IT solutions are designed from scratch and are competing with standard available products on the market</li><li>Infrastructure is established for each purpose independently and is not shared</li></ul>

### Further reading
* [IT as Manufacturing](https://atechnologyjobisnoexcuse.com/2012/10/cult-of-the-product/)

## G2 – Business value for innogy first
> **By** focusing our architecture and architectural decisions on business value to innogy as a whole, **it is ensured that** the architecture evolves to maximise the highest long-term value for the company and our shareholders, **so that** we do not seek optimum local solutions but capitalize on the best possible solution for innogy.

### Implications
* All decisions and solution designs are assessed towards benefits for the company as a whole
* Positive benefit for the whole company might have negative impact to its isolated part
* Implementation of solutions that maximize benefits for the company as a whole might be more expensive than locally oriented designs  

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Locally implemented solutions are beneficial for the whole company (or at least do not have negative impact to whole company)</li><li>Implemented solutions create value for the whole company therefore they are re-usable within the company regardless the place of origin</li><li>Consideration of benefit to the whole company is an obvious part of architecture decision making procedures</li></ul> | <ul><li>Locally implemented solutions do not create value for the whole company (or even worse have a negative impact from the whole company perspective)</li><li>Company wide benefit considerations are not part of architecture decision making procedures</li></ul> |

### Further reading
* [THINK ENTERPRISE FIRST](http://www.biske.com/blog/?p=878)

## G3 – Commit to common EAM approach
> **By** building a common Enterprise Architecture Management capability and working as a company wide IT architecture community, **it is ensured that** cross-segment transparency is established to support capability and information sharing, **so that** common information transparency challenges (for example around security, infrastructure, service management) can be centrally served and the re-use principle is supported.

### Implications
* Ownership of EAM is not with a central team, but the different architects define a common minimum data model and use a central tool to consolidate information
* The central tool is integrated into our processes – EAM is successful when the information is actively used within our processes (CMDB, Billing, Service Management, …)
* Segment IT can adopt the central tool (Renewables, Corporate, potentially Retail) or continue to use existing tools (ARIS in case of Grid) if they desire, as long as an automated integration to the central tool is in place

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Segment architects together with central EA team contributes together to create common EA capability</li><li>Agreed level of transparency about IT assets in segment IT is achieved for cross-segment purposes</li><li>IT processes benefit out of the available information from all segments IT (impact analysis, lifecycle management, etc.)</li></ul> | <ul><li>​​Different levels of transparency about IT assets exist in individual segments</li><li>​​​​Sharing capabilities and information is complicated due to fragmented information silos and lingos</li><li>Synergies are achieved by coincidence and re-use is limited​</li></ul> |

### Further reading
* TBD

# Applications and Integration

## A1 – Mesh App & Service architecture (MASA) for scaling digital business models
> **By** creating cloud-native, web-scale, modular and adaptive solutions that can be continuously and rapidly modified and refactored **it is ensured that** we have an architecture that supports growth and a rapid pace of change, that we keep strong integration capabilities with partners, ecosystems and other product lines, balancing the demand for agility and scalability of services with composition and reuse of services **so that** our architecture can meet business demands and provides a solid foundation for new digital business ecosystems.

### Implications
* The distributed nature of MASA can generate increased operational complexity, but it improves agility and scalability, which are primary requirements for any digital business.
* The classical three layered architecture is deconstructed from the individual application level to the overall IT landscape - systems are architected as a mesh of independent and loosely coupled back-end services and presentation layers are realized by web or mobile based apps
* Roadmap of digital transformation journey is developed. Application portfolio is assessed and critical applications are identified to be rearchitected to MASA.

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Applications by default support a broad range of UIs running on an array of different client devices, including PCs, tablets, smartphones, watches, kiosks, car dashboards, GPS devices and media players</li><li>Concept of layered applications (monolithic, one size fits all, layers tightly bound) is replaced by new concept of apps (non-linear interconnected mesh of independent apps and services) to provide a more optimized user experience</li><li>New applications are no longer developed as monoliths</li></ul> | <ul><li>Applications are designed in a monolithic, linear model in which an application supports one primary client interface: a browser</li><li>Operational complexity increases without getting the benefit of agility and scalability</li><li>No roadmap of application portfolio transformation exists</li></ul> |

### Further reading
* [Retire the Three-Tier Application Architecture to Move Toward Digital Business](https://www.gartner.com/binaries/content/assets/events/keywords/applications/apps20i/retire_the_threetier_applica_308298.pdf)

## A2 – Leverage platforms
> **By** designing IT solutions based on platforms (at all levels of the IT landscape), rather than just collaborating on the level of infrastructure, **it is ensured that** we can solve complex problems only once, **so that** we can be more productive and technically aligned without losing the desired level of autonomy of our segments and product teams.

### Implications
* Investigation of available platforms has to be an inevitable part of IT solution design - even across particular IT segments
* As leveraging platforms is innogy IT strategy, using platforms expects trust among teams and assumes advocacy of platforms usage beyond IT discussions
* Platforms built with the intention of re-use have to be properly documented in a shared environment so that it is easy to find such platforms while working on design of IT solutions

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Technical changes are not the issue while changing the business logic of IT solutions​</li><li>Common capabilites are quickly accessible, ready to use, secure, scalable and tested</li><li>Solutions are developed by assembly of Platform services from one or more platforms, augmented with solution specific capabilities</li></ul> | <ul><li>Every IT solution is like a snowflake - no unified approach to commodity IT exists and many tactical solutions</li><li>Productivity of DevOps teams is limited by having to deal with maintenance of their own tools</li><li>Effectiveness of IT delivery is wasted on repetitive building of commodity IT</li></ul> |

### Further reading
* TBD

## A3 – Think Cloud-First and become Cloud-Native
> **By** leveraging cloud services and developing cloud-native applications based on 12-factor methodology, **it is ensured that** we benefit from the innovation, speed, flexibility and scale of cloud services, and that we have a clear contract between applications and infrastructure, **so that** innogy has better access to technology innovation, that we can run experiments quicker and with less risk, and that our applications are more robust, scalable and flexible.

### Implications
* Organizational and cultural aspects have to be considered by development teams to follow the self-service and DevOps approach
* In case of external development or buying of development from the market, it has to be ensured that the 12-factor methodology is applied
* There may be resistance to adopting Agile and DevOps by some parts of the organization but it does not provide any reason to stop advocating this principle
* 3rd Party contracts should include provision for DevOps style of working​

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Applications offer maximum portability among execution environments</li><li>Software delivery pipelines are automated end-to-end due to increased collaboration between development and IT operations team with a shared responsibility.</li><li>Architecture of the applications is based on microservices (smaller independently deployed applications integrated together to achieve ​robustness)</li></ul> | <ul><li>Cloud computing delivery model does not bring expected benefits as its usage stays on the level of another infrastructure provider</li><li>Applications are heavily depending on underlying infrastructure (the infrastructure is not transparent)</li><li>Company will not be competitive in digital markets due to high time to market caused by low autonomy of application developers and application architecture working against agility</li></ul> |

### Further reading
* [The Twelve-Factor App](https://www.12factor.net/)

## A4 – Loose coupling is the law
> **By** avoiding design-time intersystem dependencies and by systems only being aware of their relevant contracts (semantic/structural formats, interaction flows and invariants) of services exposed by other systems, **it is ensured that** loose coupling between systems is achieved, **so that** the landscape impact of individual system changes and risks to end-to-end system integrity are significantly reduced.

### Implications
* All IT components are integrated through some integration layer (e.g. message queues) that reduce the dependency of IT components on each other
* Implementation costs of projects and changes might temporarily increase until the benefits of decreased dependencies are realised
* Data transfered by interfaces should be published in open standard formats (e.g. XML, JSON, etc.)​

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Changes of IT integration interfaces does not break the IT landscape</li><li>IT components are easily replaceable by alternative implementations providing the same services</li><li>IT maintenance complexity decrease due to independency of IT components within the IT landscape</li></ul> | <ul><li>Every change in IT integration interface must be reflected to all interface consumers so their contracts are not breached</li><li>Complexity of IT landscape changes increase with the increasing number of integrations</li><li>​​IT components are depending on underlying infrastructure and also cannot be easily replaced by alternative implementations due to high complexity and dependencies​</li></ul> |

### Further reading
* TBD

# Data and Information

## D1 – Share before replicate
> **By** preferring managed access to existing master data sources through functional services rather than replicating and duplicating an unmanaged amount of copies of the same data, **it is ensured that** overall data quality and value increases **so that** data governance is simplified and risks to process / data integrity and likelihood of data mismatches between systems are reduced.

### Implications
* Managing data in unified data sources allows the desired data quality to be maintained and minimizes wrong data usage and interpretation
* Data is exposed as functionally oriented services so other applications do not consume the data for further processing but perform the functions and present the results
* Services and their data are cataloged for easier retrieval and reuse.

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>The data is managed in defined (and unified) sources and is processed by execution of functionally oriented services</li><li>The data is not replicated between systems (if not required)</li><li>The data sources are known and documented including the data owners</li></ul> | <ul><li>The data is replicated between applications to achieve loosely coupling and reduce applications interdependence.</li><li>Services are data and not functionally oriented.</li><li>Services are used as data pumps that provide data that is then arbitrarily processed by a consumer of the service.</li></ul> |

### Further reading
* TBD

## D2 – Security by Design
> **By** applying strict information risk assessments and by embedding security controls into architecture and delivery processes, **it is ensured that** our services and systems are secure by design **so that** security does not become an expensive after-thought, customer and employee data and processes are kept secure and risk is kept to a minimum.

### Implications
* Data is classified according to its security requirements and limited work is part of company regulations.
* Data is secured in its repository during processing and protected from unauthorized access.
* Data in non-production environments is malformed or masked so that it can not be misused.

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Data is not leaked/stolen.</li><li>Only relevant data is used in processes and applications.</li><li>Data protection is par of the data processing design activities.</li></ul> | <ul><li>Data is stolen or undesirable access to sensitive data occurs.</li><li>Data is not classified according to security requirements.</li><li>It is not possible to decide whether the data is confidential or not.</li></ul> |

### Further reading
* TBD

# Technology

## T1 – Promote API-led integration
> **By** connecting data and applications through reusable and purposeful APIs in a layered approach (System, Process, Experience), **it is ensured that** we achieve higher levels of functional re-use and allow our teams to move independently, **so that** our delivery speed and flexibility increases, and our capability to integrate our products and services across internal silos and with the external world is strengthened.

### Implications
* API first thinking is changing the way of work in design and development phases - API is the first user interface of applications and should be designed independently on its implementation
* Designing API's for the system where there is no obvious demand for integration might lead to increase of implementation costs
* Integration capablity matures inside the company as people master the integration as of internal and also with external information systems

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Implementation time of projects decrease in time due to increasing ratio of re-used services</li><li>Broad availability of significant number of purposefull APIs unlocks the creativity and space for business inovation</li><li>All APIs are assorted into three categories: System, Process, Experience</li></ul> | <ul><li>Re-use of services is not easy due to the absence of purposeful APIs</li><li>APIs designs heavily depend on implementation technology that hinders general re-use</li><li>The design and documentation of APIs it not self-descriptive and easy to understood by people not involved in its creation.</li></ul> |

### Further reading
* [What is API-led Connectivity?](https://blogs.mulesoft.com/dev/api-dev/what-is-api-led-connectivity/)

## T2 – Avoid vendor lock-in
> **By** avoiding vendor-lockin through leveraging standards-based and open-source software where possible, **it is ensured that** we can switch service providers in case of cost or functional benefits without significant switching costs or inconvenience, **so that** our IT landscape remains evolvable and leverages fit-for-purpose and best of breed products.

### Implications
* Applications use the standard platforms interfaces, do not use undocumented and non-standard behavior.
* If the platform supports an open standard for implementation, it is used preferentially.
* The possibility of future technology or vendor exchange is considered during the design phase (Exit strategy).

|Successful application of the principle​|Unsuccessful application of the principle​|
|---------------------------------------|-----------------------------------------|
| <ul><li>Applications can be easily migrated to another platform and termination of platform support does not generate significant risks and costs.</li><li>Technological and vendor independence is one of the main criteria for designing the solutions</li><li>Suppliers of procured services could be easily switched.</li></ul> | <ul><li>Applications are tied to a particular technology or vendor.</li><li>Termination of technology support, price increase or dependence on suppliers generates significant risks.</li><li>Applications use non-standard platform functions.</li></ul> |

### Further reading
* TBD
