# Static Website Hosting on AWS S3 & CloudFront with Terraform

This Terraform script allows you to set up a static website hosting solution on Amazon S3 with CloudFront distribution. The CloudFront distribution provides low-latency access to your static content while taking advantage of Amazon S3's durability and scalability.

![WebHosting](https://github.com/prajapatdip/Website-Hosting/assets/104031556/6b4a8613-77f5-49be-8332-de3feb3ec539)

## Prerequisites

Before you begin, ensure you have the following prerequisites:

- [x]  [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli): Make sure Terraform is installed on your local machine.
- [X]  [AWS Account](https://aws.amazon.com/console/): Ensure you have an AWS account with the necessary permissions to create S3 buckets, CloudFront distributions, and IAM roles.

## Getting Started

#### Step 1 : Clone the Repository.

```
git clone https://github.com/prajapatdip/Website-Hosting.git
cd Website-Hosting
```

#### Step 2 : Initialize Terraform

```
terraform init
```

#### Step 3 : Configure Variables
Open the `variables.tf` file and set the required variables and other configuration options.

#### Step 4 : Review Configuration
Open `main.tf` and review the configuration. Adjust any settings according to your requirements.

#### Step 5 : Deploy Infrastructure

```
terraform apply
```

### Step 6 : Access your Website
Once the deployment is complete, you can access your website using the CloudFront distribution URL provided in the Terraform output.

## Customization

* __Website Content:__ Upload your static website content (HTML, CSS, JavaScript, images, etc.) to the S3 bucket specified in the Terraform configuration.

* __Custom Domain:__ If you have a custom domain, you can configure it with CloudFront for a more branded experience.

* __SSL/TLS:__ Customize the SSL/TLS settings in the CloudFront distribution for secure access.

## Cleanup

To avoid incurring unnecessary costs, run the following command to destroy the resources created by Terraform:

```
terraform destroy
```
