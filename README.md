# CloudGuard Native Terraform Projects

[![HIPAA](https://app.soluble.cloud/api/v1/public/badges/3798b2d3-e6de-4564-80d1-6c53d302bd63.svg)](https://app.soluble.cloud/repos/details/github.com/dasalebr/terraform-cloudguard-native)  [![CIS](https://app.soluble.cloud/api/v1/public/badges/aa4f1b1b-4c46-4f32-8bb8-02fe310200ae.svg)](https://app.soluble.cloud/repos/details/github.com/dasalebr/terraform-cloudguard-native)  [![IaC](https://app.soluble.cloud/api/v1/public/badges/b9434c9d-458e-45e5-90c2-d40a0c4df348.svg)](https://app.soluble.cloud/repos/details/github.com/dasalebr/terraform-cloudguard-native)  
# CloudGuard Native Terraform Projects
This repository is a collection of Terraform automation projects that can be used with CloudGuard Native Solution.    
hese projects are intended to be used as a template to demonstrate or build a test environment. You will find a description of what each project does in the directories, and if you want (or need) to customize them, you can change defaults in the different __*name-variables.tf*__ files. 

## Which are the projects available?
The projects can be briefly described as follows:
1. **./multiple-onboarding**: It onboards multiple Cloud accounts (Azure/AWS/GCP) and K8s Clusters in one-shot
2. **./k8s-workload**: It creates a K8s Cluster on GCP, create an application and the onboards the cluster in CloudGuard

## Do you want to see more? 
Check out my Terraform Microsoft Azure repository here: [gbrembati / terraform-azure](https://github.com/gbrembati/terraform-azure)   
Check out my Terraform Amazon Web Services repository here: [gbrembati / terraform-aws](https://github.com/gbrembati/terraform-aws)   
Check out my Terraform Google Cloud Platform repository here: [gbrembati / terraform-gcp](https://github.com/gbrembati/terraform-gcp)    
   
Check the Check Point official CloudGuard CSPM repository here: [dome9 / terraform-provider-dome9 / examples](https://github.com/dome9/terraform-provider-dome9/tree/master/examples)


## How do you use these projects?
The first thing that you need to do is download this repository, either via "*git clone*" or "*download as ZIP*".  
Choose which are projects that you want to use, and in each directory change the relative __*terraform.tfvars*__ file.   
Once you have done the above, simply go inside the directory of a single project and run these terraform commands.

##
To prepare the current working directory (and install the required providers) run :
```hcl
terraform init 
```
##
To create an execution plan (and see the changes that will be made in your environment) run :
```hcl
terraform plan
``` 
##
To apply the changes required to reach the desired state (and create your environment) run :
```hcl
terraform apply
```
## 
To destroy the Terraform-managed infrastructure, run:
```hcl
terraform destroy
```

If you want (or need) to further customize other project details, you can change defaults in the different __*name-variables.tf*__ files.
Here you will also able to find the descriptions that explains what each variable is used for.
