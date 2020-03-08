# Terraform Introduction

* Open-source infrastructure as code software tool created by [HashiCorp](https://www.terraform.io/)
* A tool for building, changing, and versioning infrastructure as code
* Almost any infrastructure type can be represented as a resource
* Cloud-specific or on-premises provider is responsible for understanding API interactions and exposing resources
* Configuration files describe the components needed whether for a server, an environment or for the entire data centre
* Execution plan describes what to is the desired state, not how to reach it
* Sample VM template for Azure cloud:
* ```
  # Azure
  resource "azurerm_virtual_machine" "web-server" {
    name                  = "web-server"
    location              = "Central US"
    resource_group_name   = "online-store-resource-group"
    vm_size               = "Standard_DS1_v2"
  }
  ```
* Terraform templates are parsed, validated and processed by a [terraform](https://www.terraform.io/downloads.html) executable on different platforms:
* `terraform validate` command parses and validates structure and content of the templates
* `terraform plan` command determines what actions are necessary to achieve the desired state of the configuration
* `terraform apply` command is used to apply the changes required to reach the desired state of the configuration
* `terraform destroy` command is used to destroy the Terraform-managed infrastructure







