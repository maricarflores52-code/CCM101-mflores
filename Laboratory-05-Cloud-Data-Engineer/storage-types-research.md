# Cloud Storage Comparison

Cloud storage has different forms depending on how information needs to be stored and accessed.

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Data is separated into blocks that can be managed individually. | Used for virtual machines, databases, and systems that need direct and fast storage access. | AWS EBS |
| File Storage | Data is kept as files and arranged through folders and directories. | Useful for shared documents, files, and applications that need a common file system. | AWS EFS |
| Object Storage | Data is stored as objects together with metadata and a unique identifier. | Suitable for photos, videos, backups, and other unstructured data. | AWS S3 |

## Why Object Storage?

Object Storage is suitable for the client's photo-sharing application because it is designed for large amounts of unstructured data. Since uploaded photos are individual files, they can be stored and accessed as objects while the storage system handles a large collection of them.
