# Types of Cloud Storage

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|--------------|-------------|------------------|------------------------|
| **Block Storage** | Splits data into fixed-size blocks, each with its own address. It works like a raw hard drive attached to a server. | Operating system disks, databases, and applications needing fast, low-latency reads and writes. | AWS EBS, Azure Managed Disks, Google Persistent Disk |
| **File Storage** | Stores data as files in a folder hierarchy that multiple servers can share over a network, like a shared network drive. | Shared folders, home directories, and content management systems. | AWS EFS, Azure Files, Google Filestore |
| **Object Storage** | Stores data as objects, each containing the data, its metadata, and a unique ID, in a flat structure of buckets. It is accessed over HTTP APIs. | Images, videos, backups, logs, and other large amounts of unstructured data. | AWS S3, Azure Blob Storage, Google Cloud Storage |

## Recommendation for the Client

Object storage is the best choice for your photo-sharing application because it scales almost without limit, so it can hold millions of user-uploaded images without you having to manage disk sizes. It is cost-effective and reachable from anywhere over the web, and each image can carry metadata such as the upload date or user ID. Because the storage is separate from your web servers, your images remain safe even when containers are stopped or replaced.
