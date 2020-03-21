# Azure IaaS

![](/assets/azure-iaas.jpg)

* The top-level container in Azure to organize our resources is a subscription across all regions
* Then a resource group as a logical container in a given region
* IaaS starts with creating an isolated from the other Azure tenants and the Internet [Virtual Network](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-overview) or VNet
* Virtual Network is not an equivalent of a single datacentre as it may span across multiple physical locations
* Virtual Network requires a network CIDR address allocation e.g. 10.0.0.0/24
* Inside a Virtual Network, one or more subnets with their own CIDR address space allocation are created
* Public subnets allow direct connectivity from the outside world, private subnets go through a gateway instead
* Traffic, inbound and outbound, and between the VM's is controlled by Network Security Group \(NSG\)
* A Virtual Machine is associated with a subnet, needs disk, protected by NSG and requires a way to access it



