# Terraform Variables

Input variables are parameters to customize a module behaviour without altering the module's own source code

Allow modules to be shared between different configurations and re-used within the same plan

```
variable "welcome_to_iac" {
  type = string
  default = "Hello World!"
}
```

Input variables can be assigned using:

```
terraform apply -var="welcome_to_iac=HelloWorld"   # on the command line
terraform apply -var-file="testing.tfvars"         # using a variables file
export TF_VAR_welcome_to_iac=HelloWorld            # using Linux shell
$env:TF_VAR_welcome_to_iac="HelloWorld"            # using Windows PowerShell
set TF_VAR_welcome_to_iac="HelloWorld"             # using Windows CMD
```

Input variables can be referenced in a terraform module:

```
...
tags {
  name = var.welcome_to_iac
}
...
```



