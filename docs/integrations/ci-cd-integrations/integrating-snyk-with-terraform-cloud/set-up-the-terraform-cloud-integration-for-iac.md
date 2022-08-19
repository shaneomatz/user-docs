# Set up the Terraform Cloud integration for IaC

## **How to set up and use the integration between Snyk and Terraform Cloud**

{% hint style="warning" %}
You must be an administrator on the Snyk organization to configure the Terraform Cloud integration.
{% endhint %}

Navigate to the dedicated Terraform Cloud integration settings page, under the **Integrations** page in the Snyk Web UI, then follow these steps:

### Set up Terraform plan scanning

On the Snyk platform, first go to the Terraform Cloud integration settings page: `https://app.snyk.io/org/{YOUR-SNYK-ORG}/manage/integrations/terraform-cloud` to access the provided URL and HMAC Key

![Snyk Integration Page for Terraform Cloud](<../../../.gitbook/assets/image (290).png>)

#### Create the Snyk Run Task for Terraform Cloud

Now navigate to [Terraform Cloud](https://app.terraform.io) in the organization global settings:

![Terraform Cloud Settings](<../../../.gitbook/assets/image (263).png>)

1. Go to the run tasks settings:\
   `https://app.terraform.io/app/{YOUR_TFC_ORG}/settings/tasks`
2. Create a new run task for Snyk with the URL and HMAC key values.\
   The HMAC key is mandatory for the Snyk integration to work, even though it is identified as optional on Terraform Cloud.

#### Associate the Run Task to your Terraform Cloud Workspace

1. Navigate to your Terraform Cloud Workspace, enter the _"Settings"_ menu and chose _"Run Tasks"_
2. The "run task" you created is available under "Available Run Tasks": click on "+" to add associate it
3. Choose the enforcement level (Advisory or Mandatory) and click Create.

Once your integration is set up, Snyk scans Terraform plans for each run triggered in your workspace.