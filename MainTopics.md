# Good Links to read for DevOps
1. [Devops](#Devops)
2. [Terraform](#Terraform)
4. [Cloud SDK, Tools and Docs](#CloudSDkToolsDocs)
5. SourceCodeManagementTools( git / svn / gitlab / bitbucket/ Cloud Source Repositories / Aws Code Commit / Azure repos)
6. Configuration management( Ansible / puppet / chef)
7. CI/CD ( Jenkins / GitActions / gcp CloudBuild /AWS CodeBuild, AWS CodeDeploy, AWS CodePipeline/ Azure Devops )
8. Iac tool ( Terraform / Pulumi / Bicep / Gcp Cloud Deployment Manager / Aws Cloud Formation / Azure Resource Manager)
9. Container Image build tools  ( Docker / Podman )
10. Container Orchestration tools ( Kubernetes / Openshift / Docker Swarm / Racher / GKE (GCE-Google Container Engine) /EKS (ECS - EC2 Container Service) / AKS (ACI - Azure Container Instance)
11. Metrics gathering, log scanning, alert and Monitoring tools ( Nagios / Grafana / prometheus / ELK / GCP Cloud Logging/Monitoring / AWS CloudWatch / Azure Monitor) 
12. Groovy / Json / xml / yaml / helm / kustomize 
13. commands find / grep / ps / vi / awk / sed / jq / chmod 

## DevOps
- [DevOps Capabilites](https://dora.dev/devops-capabilities/technical/code-maintainability/)
- [GcpDevops](https://cloud.google.com/devops)
- [AwsDevops](https://aws.amazon.com/devops)
- [AzureDevops](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-devops)
- [AtlassianDevops](https://www.atlassian.com/devops/what-is-devops/devops-culture)


## CloudSDkToolsDocs

### Aws
- [DeveloperTools](https://aws.amazon.com/developer/tools/)
- [Aws Cli](https://aws.amazon.com/cli/?pg=developertools)
- [Aws Cli Docs](https://docs.aws.amazon.com/cli/latest/userguide/welcome-resources.html)

### Azure
- [DeveloperTools](https://azure.microsoft.com/en-us/downloads/)
- [Azure Cli](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)
- [Azure Cli Docs](https://learn.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)
  
### GCP
- [DeveloperTools](https://cloud.google.com/sdk?hl=en)
- [Gcp Cli](https://cloud.google.com/cli?hl=en)
- [Gcp Cli Docs](https://cloud.google.com/sdk/gcloud/reference)

  
## Terraform 

### Terraform Aws

- [TerraformAwsProvider](https://registry.terraform.io/providers/hashicorp/aws/latest)
- [TerraformAwsProviderDocs](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
- [TerraformAwsModules](https://registry.terraform.io/search/modules?provider=aws&q=aws)
- [TerraformAwsOfficialNamespaceRegistry](https://registry.terraform.io/namespaces/terraform-aws-modules)
- [TerraformAwsOfficialNamespaceRegistryModulesList](https://registry.terraform.io/search/modules?namespace=terraform-aws-modules&provider=aws&q=aws) 
- [AwsDocs](https://docs.aws.amazon.com/index.html)
- [TerraformAwsOfficialModuleRepos](https://github.com/terraform-aws-modules)
- [AswSamples](https://github.com/aws-samples)

In below example we will be searching for service eks related all stuff in aws, terraform resource and any terraform module that can be levearaged:
- [AwsDocs](https://docs.aws.amazon.com/index.html) in all products search for [eks](https://docs.aws.amazon.com/eks/?icmpid=docs_homepage_containers)
- [TerraformAwsProvider](https://registry.terraform.io/providers/hashicorp/aws/latest) click on "**Documentation**" on top left (overview / Documentation / Use provider) and search for eks. This give all information needed for terraform resource.
- [TerraformAwsModules](https://registry.terraform.io/search/modules?provider=aws&q=aws) this give list of all modules official and other sources. But we will be concentrating on official ones. Click on any aws official module then look for published by on top left "**Published   December 15, 2023 by terraform-aws-modules**" and click on link next to it. It then lands to official modules by aws in aws namespace  [TerraformAwsOfficialNamespaceRegistry](https://registry.terraform.io/namespaces/terraform-aws-modules). click on view more to look at complete list. 
- [TerraformAwsOfficialNamespaceRegistryModulesList](https://registry.terraform.io/search/modules?namespace=terraform-aws-modules&provider=aws&q=aws)
  
Look for [eks](https://registry.terraform.io/modules/terraform-aws-modules/eks/aws/latest) module in list.
  
Look for Source code link "**Source Code: github.com/terraform-aws-modules/terraform-aws-eks**" and click to look at the code in detail related to eks.

Also checkout the examples within it if any as it could good starting point.
 
Pay attention to query in link below it uses namespace and provider 
"https://registry.terraform.io/search/modules?namespace=terraform-aws-modules&provider=aws&q=aws"

### Terraform Azure

- [TerraformAzureProvider](https://registry.terraform.io/providers/hashicorp/azurerm/latest)
- [TerraformAzureProviderDocs](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs)
- [TerraformAzureModules](https://registry.terraform.io/browse/modules?provider=azure)
- [TerraformAzureOfficialNamespaceRegistry](https://registry.terraform.io/namespaces/Azure)
- [TerraformAzureOfficialNamespaceRegistryModulesList](https://registry.terraform.io/search/modules?namespace=Azure&provider=azure) 
- [AzureDocs](https://learn.microsoft.com/en-us/azure/?product=popular)
- [TerraformAureOfficialModuleRepos](https://github.com/Azure)
- [Auzre-dat-labs-modules](https://github.com/Azure/azure-data-labs-modules) official git repo for terraform modules for all azure services

In below example we will be searching for service azure functions related all stuff in azure, terraform resource and any terraform module that can be levearaged:
- [AzureDocs](https://learn.microsoft.com/en-us/azure/?product=popular) in all products select compute and click [Azure Function](https://learn.microsoft.com/en-us/azure/azure-functions/)
- [TerraformAzureProvider](https://registry.terraform.io/providers/hashicorp/azurerm/latest) click on "**Documentation**" on top left (overview / Documentation / Use provider) and search for eks. This give all information needed for terraform resource.
- [TerraformAzureModules](https://registry.terraform.io/browse/modules?provider=azure) this give list of all modules official and other sources. But we will be concentrating on official ones. Click on any azure official module then look for published by on top left "**Published June 6, 2023 by Azure**" and click on link next to it. It then lands to official modules by aws in aws namespace [TerraformAzureOfficialNamespaceRegistry](https://registry.terraform.io/namespaces/Azure). click on view more to look at complete list. 
- [TerraformAzureOfficialNamespaceRegistryModulesList](https://registry.terraform.io/search/modules?namespace=Azure&provider=azure) 
  
Pay attention to query in link below it uses namespace and provider 
"https://registry.terraform.io/search/modules?namespace=Azure&provider=azure"



### Terraform GCP

- [TerraformGcpProvider](https://registry.terraform.io/providers/hashicorp/google/latest)
- [TerraformGcpProviderDocs](https://registry.terraform.io/providers/hashicorp/google/latest/docs)
- [TerraformGcpModules](https://registry.terraform.io/browse/modules?provider=google)
- [TerraformGcpOfficialNamespaceRegistry](https://registry.terraform.io/namespaces/terraform-google-modules)
- [TerraformGcpOfficialNamespaceRegistryModulesList](https://registry.terraform.io/search/modules?namespace=terraform-google-modules&provider=google) 
- [GcpDocs](https://cloud.google.com/docs)
- [TerraformAwsOfficialModuleRepos](https://github.com/terraform-aws-modules)
- [TerraformOnGcpDoc](https://cloud.google.com/docs/terraform)
- [TerraformGcpBlueprints](https://cloud.google.com/docs/terraform/blueprints/terraform-blueprints)
- [TerraformSampleCodes](https://cloud.google.com/docs/terraform/samples) 
  
Pay attention to query in link below it uses namespace and provider
"https://registry.terraform.io/search/modules?namespace=terraform-google-modules&provider=google"
  



## Blogs
### side vblogs
https://jayendrapatil.com/

