# Block Storage

[High-performance block storage at any scale](https://www.oracle.com/cloud/storage/#rc30p1)

We've designed our storage platform as an ideal complement to Oracle compute and networking services to support the highest performance requirements. OCI Block Volume uses the latest NVMe SSDs and provides nonblocking network connectivity to every host. Oracle delivers a consistent, low-latency performance of up to 225 IOPS/GB to a maximum of 300,000 IOPS and 2,680 MB/sec of throughput per volume.


# Table of Contents

1. [Team Publications](#team-publications)
2. [Useful Links](#useful-uinks)
3. [Reusable Assets Overview](#reusable-assets-overview)

## Team Publications

- [OCI provides native high availability and data resilience](https://blogs.oracle.com/cloud-infrastructure/post/oci-provide-cloud-resilience-by-default)
    - Blog: Oracle Cloud Infrastructure (OCI) provides high data durability and availability as a core feature, enabling businesses to concentrate on their customer experience and economic success.
- [Make your cloud resilient against regional outages](https://www.youtube.com/watch?v=IVqLe_XH_AE)
    - 6-minute Video about "Make your cloud resilient against regional outages"
- [Effortless Cloud Resilience – Automate your Disaster Recovery with Oracle Cloud Infrastructure](https://www.youtube.com/watch?v=P3qWyjE9HMQ)
    - 1h Video about "Effortless Cloud Resilience – Automate your Disaster Recovery with Oracle Cloud Infrastructure"

## Useful Links

- [OCI Block Storage documentation](https://docs.oracle.com/en-us/iaas/Content/Block/home.htm)
  - Oracle Block Storage documentation
- Introduction to Oracle Cloud Infrastructure Block Volume [Part 01](https://www.youtube.com/watch?v=rNrBxdDC8vc) and [Part 02](https://www.youtube.com/watch?v=ldZDySWv8sw)
  - Short Videos to introduce Oracle Cloud Infrastructure Block Volume
- [OCI Block Storage on oracle.com](https://www.oracle.com/cloud/storage/block-volumes/)
  - Oracle Cloud Infrastructure (OCI) Block Volumes provide reliable, high-performance, low-cost block storage. OCI Block Volumes persist beyond the lifespan of a virtual machine, have built-in redundancy, and can scale to 1 PB per compute instance.
- [Blogs on Block Storage](https://blogs.oracle.com/authors/max-verun)
  - See all Block Storage Blogs from Oracle's Product Management
- [Block Storage Release Notes](https://docs.oracle.com/en-us/iaas/releasenotes/services/blockvolume/)
- [Block Volumes FAQ](https://www.oracle.com/cloud/storage/block-volumes/faq)
- [Oracle Cloud Infrastructure Service Level Agreement (SLA)](https://www.oracle.com/cloud/sla/)
  - Enterprises demand more than just availability from their cloud infrastructure. Mission-critical workloads also require consistent performance, and the ability to manage, monitor, and modify resources running in the cloud at any time. Only Oracle offers end-to-end SLAs covering the performance, availability, and manageability of services.
- [Oracle PaaS and IaaS Public Cloud Services Pillar Document Block Storage](https://www.oracle.com/assets/paas-iaas-pub-cld-srvs-pillar-4021422.pdf#page=28)
  - Oracle offers end-to-end SLAs covering performance, availability, and manageability. Here you find details regarding Block Storage.
- [Oracle PaaS and IaaS Universal Credits Service Descriptions - Storage section](https://www.oracle.com/us/corporate/contracts/paas-iaas-universal-credits-3940775.pdf#page=178)
  - OCI Block Storage Service Description
- [Resilience and Continuous Availability of Oracle Cloud Infrastructure Services and Platform FAQ](https://www.oracle.com/cloud/iaas/faq.html)
  - Resilience and Continuous Availability FAQs
- [Oracle Cloud Infrastructure Vault: Block Volume Encryption](https://www.youtube.com/watch?v=3GBPIx4hlRU)
 - This video helps you to encrypt a block volume with the KMS Vault customer-managed encryption key.

## Reusable Assets Overview

- [Cloud Resilience](https://gitlab.com/hmielimo/cloud-resilience/-/blob/main/doc/cloud.resilience/README.md)
  - All details regarding storage-based resiliency incl. example backup and recovery automation script
- [Cloud Resilience by default](https://gitlab.com/hmielimo/cloud-resilience-by-default/)
  - All details regarding storage-based Server resiliency incl.
    - Set up your Server with Resilience by default Using the Console
    - Set up your Server with Resilience by default using CLI
    - Performance-Based Auto-tune Use Case script
- [OCI Storage Health-Check](https://gitlab.com/hmielimo/oci-storage-health-check/)
  - Storage Health-Check example scripts
    - validate all boot and block volumes regarding backup policies
    - showcase boot and block volume security e.g. using Customer managed key, Key-Rotation, Backup
- [TRIM showcase - example script](asset/trim.showcase.txt)
- [boot/block volume security best practice - example script](asset/secure.storage.sh)
- [boot/block volume individual (to a customer-managed bucket) backup and restore  - example script](asset/block.volume.backup.and.restore.txt)



# License

Copyright (c) 2023 Oracle and/or its affiliates.

Licensed under the Universal Permissive License (UPL), Version 1.0.

See [LICENSE](https://github.com/oracle-devrel/technology-engineering/blob/folder-structure/LICENSE) for more details.
