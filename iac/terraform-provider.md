# Terraform Provider

* Responsible for interacting with provider-specific API's
* Responsible for understanding API interactions and exposing resources
* Generally are IaaS \(infrastructure as a Service\) e.g. Alibaba Cloud, AWS, GCP, Microsoft Azure, OpenStack 
* Some PaaS \(Platform as a Service\) e.g. Heroku
* And some SaaS \(Software as a Service\) e.g. Terraform Cloud, DNSimple, Cloudflare
* Azure Provider configuration:
* ```
  provider "azurerm" {
    version = "=1.38.0"
  }
  ```
* VMWare vSphere Provider configuration:
* ```
  provider "vsphere" {
    user           = "username for vSphere API operations"
    password       = "password for vSphere API operations"
    vsphere_server = "vCenter server name"
  }
  ```



