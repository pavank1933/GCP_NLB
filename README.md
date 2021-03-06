# GCP_NLB
Create nlb setup in GCP<br/>
**STEPS:** <br/>
**config.yaml-** Create VPC, Subnets, instances in the respective subnets in GCP using deployment manager scripts. <br/>
**main.yaml-** Create NLB in GCP <br/>

## Pre-requisites
#### (a)
**Gcloud deployment manager enable API setup**<br/>
https://cloud.google.com/deployment-manager/docs/step-by-step-guide/installation-and-setup

#### (b)
**Install Cloud SDK**<br/>
Download and authenticate gcloud
Alternatively, use Cloud Shell, which comes with gcloud already installed.
**Set your project ID**<br/>
gcloud config set project myproject
**Set your default zone and region**<br/>
gcloud config set compute/region region_name
gcloud config set compute/zone zone_name

#### (c) **Final step**
**Deploy the resources**<br/>
gcloud deployment-manager deployments create quickstart-deployment --config main.yaml