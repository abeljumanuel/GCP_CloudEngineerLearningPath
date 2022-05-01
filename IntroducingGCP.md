# Introducing GCP_CloudEngineerLearningPath
Notes about the course
> **Cloud Computing** is a model for enabling uniquitous, conveniente, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, apps, and services) that can b e rapidly provisioned an released with minimal management effort or service provider interaction. This cloud model is composed of **five essential characteristics**, **three service models**, and **four deployment models**. *NIST*

> Google realized that its business couldn't move fast enough within the confines of the virtualization model. So **Google switched** to a **Container-based architecture-** a fully automated, elastic third-wave cloud that consists of a combination of automated services and scalable data. 

## Characteristics
1. Customers get computing resources on-demand and self-service. **CC** customers use an automated interface and get the processing power, storage, and network they need, with no need for human intervention.
2. They can access these resources over the network
3. The provider of those resources has a big pool of them, and allocates them to customers out of the pool. That alllows the provider to get economies of scale by buying in bulk. Customers don't have to know or care about the exact physical location of those resources.
4. The resources are elastic. 
5. The customers pay only for what they use or reserve, as they go. If they stop using resources, they stop paying.

## Service Models
1. User-configured, managed, and maintened
2. User-configured, Provider-managed and Mantained
3. Fully automated

## Deployment Models
1.
2.
3.
4.



![image](https://user-images.githubusercontent.com/12539100/165638989-8ac1b93c-059a-4bcd-b4de-598b75ad7ff4.png)
> **IaaS** provide raw compute, storage and network, organized in way familiar from physical and virtualized data centers. *Pay what you allocate*
> **PaaS** on the other hand, bind the code to libraries that provide access to the infraestructure tha the apps needs, thus allow focus on the application logic. *Pay what you Use*
![image](https://user-images.githubusercontent.com/12539100/165639704-2c3338d0-5063-45bf-99d1-89d13a40325a.png)

## *GCP* is organized into regions and zones
![image](https://user-images.githubusercontent.com/12539100/165642712-f7293b1a-864f-4f42-9db2-c10b4c79e953.png)
### Regions and zones
> are independent geographic areas that consist of *zones* (Group of Countries).
> **Zones** is a deployment area for GCP resources within a region.
> Multiregion is The better way to protect against the loss of an entire region due to natural disaster, our customers should deploy apps across multiple zones in a region.

### Zonal resources
>If a zone becomes unavailable, all of the zonal resources in that zone are unavailable until service is restored.
> > *Google Compute Engine VM instance resides within a specific zone*
### Regional resources
> Are deployed with  redundancy within a region . This gives them higher availability relative to zonal resources.
### Multi-regional resources
>A few GCP service are managed by Google to be redundant and distributed within a across regions. These services optimize availability, performance, and resource efficiency
![image](https://user-images.githubusercontent.com/12539100/165644413-1af208d6-7520-4232-93c0-bf596ab45e4b.png)

## Google gives customers the ability to run their apps elsewhere if Google becomes no longer the best provider for their needs.
> Open APIs. compatible with open-source products. **Google Cloud Bigtable** uses Apache HBase interface, **Google Cloud Dataproc** offers open-sourcce big data environment Hadooop as a managed service.
> Open-Sources licences. Create ecosystems that provide customers with options other than Google. **TensorFlow** use Machine Learning developed inside Google.
> Interoperability at multiple layers of the stack. **Kubernetes & Google Kubernetes Engine** mix and match microservices running across differente clouds. *Google Stackdriver* lets customers monitor workloads across multiple cloud providers.

## Resume
![image](https://user-images.githubusercontent.com/12539100/165646416-4c3d9d6c-5970-46ad-a141-b7ba95e7fba6.png)

![image](https://user-images.githubusercontent.com/12539100/165646475-1bc83100-ca7a-4209-9734-1bfa5dd42276.png)

![image](https://user-images.githubusercontent.com/12539100/166128527-9af8e0eb-9c33-41c9-bc1b-4ca15aa4f06c.png)

## Friendly Pricing for Customers
![image](https://user-images.githubusercontent.com/12539100/166128320-8c73ef60-5091-430d-93ce-45557457aa8b.png)

## Why choose GCP?
- Enable developers to **build, test,** and **deploy** apps on Google's **highly secure, reliable**, and **scalable** infrastructure.

## About the Security by layers
1. Hardware Infraestructure: Hardware design an provenance; secure boot stack; premises security
2. Service deployment:  Encryption of inter-service communication
3. User Identity: Central identity service with support for U2F (Universal 2nd Factor)
4. Storage services: Encryption at rest
5. Internet Communication: Google Front End; designed-in Denial of Service protection
6. OPerational Security: Intrusion detection systems; techniques to reduce insider risk; employee U2F use;  software development practices

## Budgets and Billing 
- Could create alerts based on your monthly consume or customized
- Billing export let us to know a detailed analysis about a bigquery data or other resources over owr GCP
- Can implement Rate Quota or Allocation Quota
