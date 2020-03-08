# Tools & Approaches

* Configuration Orchestration designed to automated infrastructure deployment, e.g. [Terraform](https://www.gartner.com/reviews/market/cloud-management-platforms/vendor/hashicorp/product/terraform-enterprise/ratings?timeFilter=12)
* Configuration Management helps configure software on provisioned infrastructure, e.g. [Ansible](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/red_hat/product/red-hat-ansible)
* Infrastructure API/SDK are required for automation, e.g. [vSphere Automation API](https://code.vmware.com/apis/366/vsphere-automation) or [Azure API](https://docs.microsoft.com/en-us/rest/api/azure/)
* Declarative: code specifies the desired end-state, the tool resolves the discrepancy between actual and desired
* Procedural: code specifies, step-by-step, how to achieve the desired end-state
* Mutable: the servers are changed after they are provisioned
* Immutable: the servers are never modified after they’re deployed
* A [comparison](https://www.ibm.com/cloud/blog/chef-ansible-puppet-terraform) article by IBM



