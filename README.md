# Notes

## Cloud Computing and GCP Fundamentals

- **private cloud:** private cloud = on-premise cloud
  - private cloud follows the 5 characteristics of cloud
- **on-premise data center:** a group of servers that you privately own and control
  - private data center does not follow the 5 characteristics of cloud
- <kbd><img width="777" alt="Screen Shot 2023-06-24 at 5 28 01 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/8069c086-d5c6-4f73-ac9a-c4aa69641db9"></kbd>
- **Network File System (NFS):** a distributed file system protocol for shared storage. The NFS shared storage protocol defines the way files are stored and retrieved from storage devices across networks. It is one of several network-attached storage (NAS) distributed file system standards
- **IOPS:** input/output operations per second

## Account Setup

- <kbd><img width="666" alt="Screen Shot 2023-06-25 at 1 18 09 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/d5cdb801-1368-4b0a-8ea8-d5b5fa74754e"></kbd>
- **billing account:** used to track the usage and costs of GCP services, and to receive invoices or make payments for those services
- **payment profile:** a representation of a payment method used to pay for GCP services
- **billing account vs payment profile:** A billing account can have one payment profile associated with it, and a payment profile can be associated with one billing account at a time
- **workspace:** A workspace usually represents the root folder of your project and includes your project-specific configuration files
  - a workspace is a container for organizing and managing related resources, such as projects, folders, and billing accounts
  - workspaces are used to group resources together based on criteria such as business unit, department, or environment (e.g., development, testing, production)
  - with workspaces, you can specify persistent settings, run and debug configurations, and UI states (like open files) for all the folders in your workspace
- <kbd><img width="666" alt="Screen Shot 2023-06-26 at 11 06 26 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/20c0ff57-fdec-4945-ac40-ba323867b134"></kbd>

## Identity and Access Management

- <kbd><img width="666" alt="Screen Shot 2023-06-27 at 5 16 32 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/d7d6ad7a-605b-41ae-b6af-3c12e90a39ef"></kbd>
- <kbd><img width="666" alt="Screen Shot 2023-06-27 at 5 24 09 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/dd455445-8fb8-4b62-9a50-130a5ed0d0bc"></kbd>
- <kbd><img width="666" alt="Screen Shot 2023-06-27 at 6 03 03 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/c9f10b87-268f-4f7a-9481-bf3026c29b7f"></kbd>
- **Google Cloud Directory Sync (GCDS)**
  - <kbd><img width="1433" alt="Screen Shot 2023-06-27 at 6 49 16 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/d51443db-c566-45b4-a4b7-fb8e43bbe570"></kbd>

## Networking Services

- **subnetting:**
  - the process of dividing a network into smaller networks
  - the number of the perfix will increase each time you subnet
- The subnet IP address range within a VPC in GCP is typically private IP addresses
- <kbd><img width="777" alt="Screen Shot 2023-06-28 at 1 15 06 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/8d9b4a04-1ac6-4cac-9c33-06932bf1ec07"></kbd>
- **private google access:**
  - a feature in GCP that allows instances within a VPC network to access Google APIs and services using private IP addresses, without requiring public IP addresses or internet access
- <kbd><img width="666" alt="Screen Shot 2023-06-28 at 1 24 03 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/ee96be7c-6ff2-4bd3-b707-41e422025fb1"></kbd>
- **internal IP address reservation:**
  - when you reserve an internal IP address, it guarantees that the IP address will be available for use by your instances or other resources within the VPC
  - when you reserve an IP address, it becomes `static` as shown in the above graph 










# Google Cloud Associate Cloud Engineer  

Course Files for Google Cloud Associate Cloud Engineer Course by Antoni Tzavelas

If you feel that something should be corrected or updated please reach out and let me know at antoni@antonit.com

If you are looking to help me with a fix, feel free to submit a PR with your suggested fixes and I will kindly review it.
