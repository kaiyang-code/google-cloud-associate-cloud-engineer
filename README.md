# Notes

## Cloud Computing and GCP Fundamentals

- **private cloud:** private cloud = on-premise cloud
  - private cloud follows the 5 characteristics of cloud
- **on-premise data center:** a group of servers that you privately own and control
  - private data center does not follow the 5 characteristics of cloud
- <kbd><img width="666" alt="Screen Shot 2023-06-24 at 5 28 01 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/8069c086-d5c6-4f73-ac9a-c4aa69641db9"></kbd>
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
  - <kbd><img width="666" alt="Screen Shot 2023-06-27 at 6 49 16 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/d51443db-c566-45b4-a4b7-fb8e43bbe570"></kbd>

## Networking Services

- **subnetting:**
  - the process of dividing a network into smaller networks
  - the number of the perfix will increase each time you subnet
- The subnet IP address range within a VPC in GCP is typically private IP addresses
- <kbd><img width="666" alt="Screen Shot 2023-06-28 at 1 15 06 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/8d9b4a04-1ac6-4cac-9c33-06932bf1ec07"></kbd>
- **private google access:**
  - a feature in GCP that allows instances within a VPC network to access Google APIs and services using private IP addresses, without requiring public IP addresses or internet access
- <kbd><img width="666" alt="Screen Shot 2023-06-28 at 1 24 03 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/ee96be7c-6ff2-4bd3-b707-41e422025fb1"></kbd>
- **internal IP address reservation:**
  - when you reserve an internal IP address, it guarantees that the IP address will be available for use by your instances or other resources within the VPC
  - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 1 35 52 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/e96a59a8-7a93-4ddf-b8de-c89b0c739c6e"></kbd>
- **external IP address reservation:**
  - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 1 38 14 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/d8bf274a-ee9a-4ca9-bbc3-7169604d033d"></kbd>
- To allow ingress traffic from VM instances in a peer network, you must create ingress allow firewall rules. By default, ingress to VMs are blocked by the **implied deny ingress rule**
  -  <kbd><img width="666" alt="Screen Shot 2023-06-28 at 2 21 47 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/9439c6d2-ba67-4b66-a84b-59a8805a5fdf"></kbd>
- **Shared VPC**
  - **single host shared vpc:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 2 38 33 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/4a7dab60-61e2-4edf-857a-5b02935ae9ec"></kbd>
  - **multi-host shared vpc:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 2 39 57 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/cc6ee8eb-b7c4-4d0f-9bf9-5500d13c693b"></kbd>
  - **hybrid enviornment:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 2 42 52 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/2ad3dc2b-83ae-4e8c-ba83-9b9e0f183b41"></kbd>
  - **two-tier web service:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 2 44 13 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/c4c835be-8f78-4792-9d7e-64cbd09bf6a9"></kbd>
- **DNS (Domain Name System):**
  - **zone:** a zone is a container of DNS records that are queried by DNS
  - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 3 30 13 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/3f4745cf-4a4f-4441-8cdb-cf1852f6d506"></kbd>
  - <kbd><img width="666" alt="Screen Shot 2023-06-28 at 3 30 54 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/b3a996d4-8752-4b29-859e-2f3b16db0a3a"></kbd>
  - **TTL:**
    - TTL stands for Time to Live in the context of DNS (Domain Name System). It is a value specified in DNS records that indicates the length of time, in seconds, that a DNS resolver or caching server should store the information before considering it expired and requesting a fresh copy from the authoritative DNS server
- **NAT (Network Address Translation)**
  - **Port Address Translation (PAT):** this type of NAT is where multiple private IP addresses are translated using a single public IP address and a specific port
    -  <kbd><img width="666" alt="Screen Shot 2023-06-29 at 4 27 22 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/02fe36c6-e7ac-4007-a78e-cf51ee892ed8"></kbd>
  -  **Static NAT:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-29 at 4 15 53 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/245e30fb-ca3a-4176-b9af-8615c7c63e5f"></kbd>
  - **Dynamic NAT:**
    - <kbd><img width="666" alt="Screen Shot 2023-06-29 at 4 23 14 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/02b5d2df-90a3-46c4-9d42-9bc1cdeefc06"></kbd>

## Compute Engine

- **Persistent Disk** and **Local SSD** are the two available types of block storage devices in Google Cloud
- **instance life-cycle:**
  -  <kbd><img width="666" alt="Screen Shot 2023-06-30 at 4 05 41 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/7dcc979b-6677-4df0-b9ab-9daa4ed4fdda"></kbd>
- **Persistent Disk & Local SSD:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 1 24 09 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/129cf98a-9f79-400c-ab68-5a12ba2a7d17"></kbd>
- **snapshots:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 11 36 04 AM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/a678b0bf-5740-42a7-898d-ff92be234917"></kbd>

## High Availability and Autoscaling

- **Load Balancing Type:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 15 20 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/8cc214c0-48d4-4458-ba8a-336da89efbb8"></kbd>
  - **Session Affinity:** a technique used in load balancing to ensure that requests from a client are consistently routed to the same server or instance for the duration of a session
  - **Service Timeout:** a parameter used in load balancing to determine how long a load balancer should wait for a response from a server or instance before considering it unresponsive or timed out
  - **Backend service:** defines how Cloud Load balancing distributes traffic, the backend services configuration contains a set of values such as the protocol used to connect to the backend, various distribution in session settings, health checks, and timeouts\
  - **Network Endpoint Group (NEG):** a configuration object that specifies a group of backend endpoints or services and a common use case for this configuration is deploying into containers
- **HTTP(S) Load Balancer:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 38 33 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/6e5a95a5-f9a9-401f-bc92-cf26897e41e7"></kbd>
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 39 32 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/83c63cdf-d336-4d84-b257-5f2d4168e4f6"></kbd>
- **SSL Proxy**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 41 21 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/01ce12ab-e662-4169-a47c-b81b24fb431a"></kbd>
- **TCP Proxy**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 43 50 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/7a34c59a-00eb-49ad-a686-0a2f9b15c234"></kbd>
- **Network Load Balancer**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 44 44 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/541ee4a1-0bc4-4fb8-a45b-b36ca218cb0a"></kbd>
- **Internal Load Balancer**
  -  <kbd><img width="666" alt="Screen Shot 2023-07-01 at 12 45 18 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/91e4ab18-9494-45d1-bd28-fe4b43261e62"></kbd>

## Kubernetes Engineer and Containers

- **VM vs Containers:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 09 18 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/cabce042-1fb0-409c-8ef2-2b81ff4d2aaa"></kbd>
- **docker image:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 11 30 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/17080923-d9ef-43a1-88ec-17df47c8219c"></kbd>
- **docker container:**
  - a read/write layer is created on top of the docker image everytime a docker container is running
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 14 17 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/abb55dbc-f2d1-4936-baff-db8d1bb42bb3"></kbd>
- **GKE**
  - the control plane is always upgraded before the nodes
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 24 33 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/e5bdb6c2-fc19-40e7-9c4c-6e28ccff0f27"></kbd>
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 41 30 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/5ecfc092-462e-4142-850a-98e6f6b1f54c"></kbd>
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 2 42 26 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/51910135-b059-481e-a587-8247b5cc2402"></kbd>
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 3 01 30 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/6dee9e16-931c-45cf-8592-e50649a1b29b"></kbd>
- **Kubernetes Services:**
  - **ClusterIP:**
    - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 5 28 52 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/88d787ba-6e4f-4d46-b1af-1247a7533448"></kbd>
  - **NodePort:**
    - relies on knowing the ip addresses of the nodes, which can change at any time
    - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 5 29 54 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/f9f8d5f0-7645-47e4-a236-77f00e9c4e94"></kbd>
  - **LoadBalancer:**
    - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 5 34 42 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/0c8a09f1-15d2-403d-be3c-4f65d0ee86d6"></kbd>
  - **Multi-Port Services:**
    - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 5 39 15 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/60e2667a-7e99-4191-8b4e-169a2aa701fb"></kbd>
  - **Network endpoint groups (NEG):**
    - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 5 52 46 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/0b2ee0e3-996b-4a63-b3f5-38ea73aa5ad8"></kbd>
- **GKE Storage Options:**
  - <kbd><img width="666" alt="Screen Shot 2023-07-01 at 6 05 02 PM" src="https://github.com/kaiyang-code/google-cloud-associate-cloud-engineer/assets/57576013/f30a2527-5bbd-4466-bf4a-76c84443920a"></kbd>

## Hybrid Connectivity

- **IPsec:** short for Internet Protocol Security, is a suite of protocols and standards that provide security services for IP (Internet Protocol) network communication
- **IKE:** stands for Internet Key Exchange, is a protocol used for secure key exchange and negotiation in IPsec-based VPN (Virtual Private Network) connections




# Google Cloud Associate Cloud Engineer  

Course Files for Google Cloud Associate Cloud Engineer Course by Antoni Tzavelas

If you feel that something should be corrected or updated please reach out and let me know at antoni@antonit.com

If you are looking to help me with a fix, feel free to submit a PR with your suggested fixes and I will kindly review it.
