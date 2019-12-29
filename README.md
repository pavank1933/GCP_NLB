# GCP_NLB
Create nlb setup in GCP
**1.** Create VPC, Subnets, instances in the respective subnets in GCP using deployment manager scripts

## Pre-requisites
#### a.
**Gcloud deployment manager enable API setup**
https://cloud.google.com/deployment-manager/docs/step-by-step-guide/installation-and-setup

#### b.
**Install Cloud SDK**
Download and authenticate gcloud
Alternatively, use Cloud Shell, which comes with gcloud already installed.
**Set your project ID**
gcloud config set project myproject
**Set your default zone and region**
gcloud config set compute/region region_name
gcloud config set compute/zone zone_name

#### c.
**Deploy the resources**
gcloud deployment-manager deployments create quickstart-deployment --config vm.yaml