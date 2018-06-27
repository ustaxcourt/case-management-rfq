# DRAFT
# REQUEST FOR QUOTE #18-0018
# United States Tax Court
# Electronic Filing — Case Management System (EF-CMS)

## Appendix B

**Tax Court Network Environment**

The Court maintains a data network that operates in a Windows environment and supports approximately 250 internal users.  The Court currently contracts with Iron Bow Technologies, LLC for a broad variety of network-related services.

The Court’s future EF-CMS will have three virtualized environments:

- A Development Environment that will support software configuration, custom-development, data migration, and test case/data creation.

- An Internet-connected Staging Environment.

- An Internet-connected Production Environment (with a standby COOP/DR instance located in a geographically distant location).

It will be the responsibility of an EF-CMS Contractor to provide and maintain its own development environment.  The Court will provide the internet-connected staging and production environments.  Offerors must state in their quote whether additional hardware, software or ancillary equipment is required for the development, staging, or production environments, and provide details including associated estimated costs.

The Court monitors and manages application performance using Cisco AppDynamics.  The Court is in the process of moving to a hierarchical file storage solution based on Commvault.  The Court expects that the hardware and software comprising the EF-CMS will either be located on premise, or on a FedRAMP-certified cloud storage solution controlled by the Court, or some hybrid thereof.

Internal Tax Court users access the network using Court-issued devices including desktops (currently Windows 10), laptops (currently Windows 10), tablets, and/or smartphones.  For remote access, internal users use a VPN on Court-issued devices, and the Court plans to introduce a Virtual Desktop Interface (VDI) for remote access, including for Bring Your Own Devices (BYOD).

Outside the Washington, DC headquarters location, the Court leases field courtroom space in 37 cities throughout the nation.  These sites use a combination of T1 and 4G connections to the Washington, D.C. headquarters location, meaning that these sites can be bandwidth-constrained, and Cisco’s Wide Area Application Services to enhance the remote site connections.

The Court has a Nutanix hyper-converged environment.  The Nutanix hardware platform has redundant power supplies, memory, and can withstand multiple hard disk failures.  All nodes within the system work together as a cluster.  All Nutanix servers utilize Windows Server 2012 R2.

The Court’s current network system is configured in a single instance Microsoft SQL Server Cluster, with SQL and Windows failover clustering (SQL Failover Cluster Interfaces and Windows Server Failover Clustering).  The Court has a disaster recovery offsite location, with Nutanix replication and AlwaysOn Availability Groups, which replicates the primary database to a secondary database at the disaster recovery site.

Tables 1 and 2 below provide information on the Court’s current SQL Server and VM Server environment (servers, cores, memory, and disk storage).

**Table 1 - SQL Production Server Specifications**

| **# Cores** | **Memory** | **Comments** | **Disk** |
| --- | --- | --- | --- |
| 4 | 64GB | SQL 2016 | C: 256GB, D: 256GB, E:Databases1 – 3TB, F:Databases2 – 3TB, G:Databases3 – 3TB, H:TempDB1 – 50GB, I:TempDB2 – 50GB, J:UserDBLogs – 100GB, K:TempDB Logs – 50GB, Q:Quorum – 2GB, X:CD |
| 4 | 64GB | SQL 2016 |   |
| NA | NA | Microsoft SQL Failover Cluster (FCI) |   |
| NA | NA | Microsoft Failover Cluster (not SQL). Needed for SQL Clustering |   |
| NA | NA | Part of Microsoft Failover Cluster (not SQL). Needed for SQL Clustering |   |
| 4 | 64GB | SQL 2016 | C: 256GB, D: 256GB, E:Databases1 – 3TB, F:Databases2 – 3TB, G:Databases3 – 3TB, H:TempDB1 – 50GB, I: TempDB2 – 50GB, J:UserDBLogs – 100GB, K:TempDB Logs – 50GB, Q:Quorum – 2GB
X:CD |



**Table 2 - VM Server Specifications**

| **# Cores** | **Memory** | **Comments** | **Disk** |
| --- | --- | --- | --- |
| 6 | 64GB |   | C:OS - 256G D:SWAP & WORK – 256GB E:DATA – 200GB X:CD |
| 4 | 6 |   | C: 160GB |
| 4 | 6 |   | C: 160GB |
| 4 | 6 |   | C: 160GB |
| 4 | 6 |   | C: 160GB |
| 4 | 6 |   | C: 160GB |
| 12 | 144 | Physical machine inside the DMZ that hosts the two Hyper-V Web servers | C: 1TB |
| 4 | 16 | Hyper-V | C:OS – 200GB D:SWAP & WORK – 200GB
E:DATA – 300GB X:CD |
| 4 | 16 | Hyper-V | C:OS – 200GB D:SWAP & WORK – 200GB
E:DATA – 300GB X:CD |
