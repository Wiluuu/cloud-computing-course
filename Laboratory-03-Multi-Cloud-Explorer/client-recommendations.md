# Client Cloud Recommendations

## Scenario Analysis & Recommendations

### Client A – Startup Company
- **Recommended Platform:** Amazon Web Services (AWS)
- **Explanation:** AWS provides extensive free-tier access, startups credits (AWS Activate), and immense scalability suited for rapid expansion. Its flexible pay-as-you-go pricing allows a cost-constrained startup to launch quickly without high upfront infrastructure investments. As the mobile application user base grows rapidly, AWS components scale seamlessly to meet demand.
- **Recommended Services:** Amazon Lightsail / EC2, Amazon S3, Amazon Cognito.

---

### Client B – University
- **Recommended Platform:** Microsoft Azure
- **Explanation:** Azure provides direct compatibility with the university's existing infrastructure, such as Active Directory, Windows Server, and Microsoft 365. Migrating to Azure minimizes migration friction and reduces retraining costs for the IT department. Additionally, Microsoft offers unified identity management through Microsoft Entra ID and beneficial academic licensing options.
- **Recommended Services:** Azure Virtual Machines, Microsoft Entra ID, Azure SQL Database.

---

### Client C – AI Research Company
- **Recommended Platform:** Google Cloud Platform (GCP)
- **Explanation:** GCP leads the industry in data analytics, custom machine learning hardware (TPUs), and artificial intelligence tooling like Vertex AI. The platform is optimized for compute-intensive research workloads requiring fast data pipelines and high-performance tensor operations. GCP provides specialized AI frameworks and scalable infrastructure tailored specifically for data science applications.
- **Recommended Services:** Google Compute Engine (GPU/TPU instances), Vertex AI, Google Cloud Storage.

---

### Client D – Global E-Commerce Company
- **Recommended Platform:** Amazon Web Services (AWS)
- **Explanation:** AWS possesses an unmatched global network footprint with robust auto-scaling capabilities and high availability features across multiple geographic regions. Its mature traffic distribution and edge-caching solutions ensure fast load times and uninterrupted shopping experiences for international shoppers. E-commerce platforms benefit significantly from AWS's proven stability during massive peak-traffic sales events.
- **Recommended Services:** Amazon EC2 with Auto Scaling, Amazon CloudFront (CDN), Amazon DynamoDB.

---

## Multi-Cloud Decision Matrix (Checkpoint 6)

| Business Requirement | Recommended Platform | Justification |
| :--- | :--- | :--- |
| **Startup Company** | AWS | Cost-effective scaling, strong free tier, and startup support programs. |
| **Enterprise Organization** | Azure | Hybrid cloud flexibility and seamless migration for legacy architectures. |
| **Microsoft Environment** | Azure | Native compatibility with Windows Server, Active Directory, and M365. |
| **AI / Machine Learning** | GCP | Native TPU support, advanced BigQuery analytics, and Vertex AI suite. |
| **Kubernetes Deployment**| GCP | Industry-leading managed Kubernetes experience via native GKE. |
| **Global Web Application**| AWS | Proven multi-region resilience, low-latency CDN, and automated elasticity. |
