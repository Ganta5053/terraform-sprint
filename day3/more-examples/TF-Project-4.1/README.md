# Introduction 
 This is the terraform script to create RG and storage account,FunctionApp using module

# Folder Structure
 	main 
        main -> which has main terraform scripts
        variables -> is having all the variables and default values
        providers.tf -> is having all the providers required
        README.md -> is containing all the help
    modules  -> will have all the sub folders where respetive modules are written
        appserviceplan
        functionapp
        resourcegroup
        storageaccount

# Pre-requisites
   1. Need to have Azure service principal -> with contributor role is assigned
   2. Set below envirnment variables
	    ARM_TENANT_ID
	    ARM_SUBSCRIPTION_ID
	    ARM_CLIENT_ID
	    ARM_CLIENT_SECRET

# Terraform commands
    - Run all the terraform commands from tf_main folder
    - No need to import/reference. With in the folder, terraform understands and reads all the .tf files
    ---------
    terraform init
    terraform validate
    terraform plan
    terraform apply
    terraform destroy
    ---------