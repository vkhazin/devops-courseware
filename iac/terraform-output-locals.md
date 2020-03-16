# Terraform Output & Locals

* Output values are like return values from a function, in Terraform terms, from a module
* ```
  output "sql_server_private_ip" {
    value = azure_instance.sql-server.ip_address
  }
  ```
* To read output value using a command line: `terraform output sql_server_private_ip`
* Local value assigns a name to an expression or a [function](https://www.terraform.io/docs/configuration/functions.html) to be used multiple times within a module or a plan
* ```
  locals {
    created_timestamp = "${timestamp()}"
  }
  ```
* There is no mechanism to read/write a local variable, a combination of a local variable with an input/output variable is ok





