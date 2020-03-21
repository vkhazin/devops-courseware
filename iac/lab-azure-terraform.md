# Lab: Terraform for Azure IaaS

* Navigate to [https://shell.azure.com](https://shell.azure.com) a personal account with full control is required
* Login with Microsoft Credentials
* Initialize Azure Shell and required storage account
* Once the shell has loaded, select PowerShell, and select the double parenthesis icon to open the editor
* In the terminal pane clone git repository: `https://github.com/vkhazin/terraform-azure-windows-courseware.git`
* Let's review the files and ask questions as we go
* `variables.tf`: input and output variables for the templates
* `./envs/azure-poc.tfvars` values for the input variables
* `provider.tf`: azure provider configuration
* `resource-group.tf`: the top-level resource organizer in a given region
* `network.tf`: resources required to create a network
* `sqlserver-vm.tf`: resources required to launch a new Windows Server 2016 with additional disks attached
* In the `readme.md` you will find instructions to make use of the templates
* Review, validate, apply the changes and login into the newly created VM using Remote Desktop
* Once satisfied with the results destroy the deployment to avoid accumulating charges to your subscription



