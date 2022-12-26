# Cloud Foundation Toolkit (CFT)
aka **Terraform blueprints**

## 0. [terraform-google-bootstrap](https://github.com/terraform-google-modules/terraform-google-bootstrap) 
aka CFT Bootstrap module
- help bootstrap a GCP organization, creating all the required GCP resources & permissions
- semi-automate and mannual

The bootstrap step includes 2 projects
- `prj-b-seed`: stores Terraform state (in bucket) and has the service accounts that can create or modify infrastructure.
- `prj-b-cicd`: the deployment of that infrastructure is coordinated by your CI/CD tool(Cloud Build or Jenkins)


## [1. org](https://github.com/terraform-google-modules/terraform-example-foundation#1-org)
Terraform code is deployed by your chosen CI/CI tool in step [0. bootstrap](#0-bootstrap-semi-automate)
