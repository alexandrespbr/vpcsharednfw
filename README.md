# vpcsharednfw
Deploy Multi-Account VPC Sharing with Network Firewall

AWS customers begin by building resources in a single AWS account that represents a management boundary which segments permissions, costs, and services. However, as the customer’s organization grows, greater segmentation of services becomes necessary to monitor costs, control access, and provide easier environmental management. A multi-account solution solves these issues by providing specific accounts for IT services and users within an organization. AWS provides several tools to manage and configure this infrastructure including AWS Landing Zone and AWS Control Tower.

Customers can use two different VPC flow patterns to set up multi-VPC environments: many-to-many, or hub-and-spoke. In the many-to-many approach, the traffic between each VPC is managed individually between each VPC. In the hub-and-spoke model, all inter-VPC traffic flows through a central resource, which routes traffic based on established rules, in this model we will follow the hub-spoke approach.

AWS Network Firewall is an AWS managed network firewall service for a VPC. It provides advanced filtering (including domain name filtering) and intrusion prevention capabilities. AWS Network Firewall does not replace, but complements Network ACLs and Security Groups. It includes both stateless and stateful filtering capabilities, whereby stateful rules are compatible to with Snort and Suricata.
