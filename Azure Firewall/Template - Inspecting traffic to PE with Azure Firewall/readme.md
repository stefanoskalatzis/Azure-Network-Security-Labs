## Warning

Check the Azure KeyVault within the newly created Resource Group, then go to Secrets to gain access to the usernames and passwords required for logging into the Windows VM and the MySQL instance.

## Pre-requisites:
1. Configure your Terraform environment. Example using Terraform on Windows with PowerShell: https://learn.microsoft.com/en-us/azure/developer/terraform/get-started-windows-powershell?tabs=bash
2. Download the main.tf file

## Recommended TF Commands:
1. terraform init
2. terraform plan -out main.tfplan
3. terraform apply main.tfplan
