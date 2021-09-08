![DH/N2 Logo](https://sdg-appstore-images.s3-us-west-2.amazonaws.com/discussionHero/dh_n2.png)
# Getting started with Discussion Hero and Nebula 2 #

Discussion Hero and Nebula 2 (DH/N2) is a 2-in-1 LTI application. You will have access to both Discussion Hero and Nebula 2 after following this installation guide. 

## Requirements
* An Amazon Web Services (AWS) instance where you are able to deploy the following: Lambda Functions, Cloudfront Distributions, S3 Buckets, Cloudformation Templates.
* [NodeJS](https://nodejs.org/en/)
* [Serverless Framework](https://www.serverless.com/framework/docs/getting-started/)

### Important Note:
The Serverless Framework needs to be configured to your AWS instance by adding AWS credentials. Please see instructions here: [https://www.serverless.com/framework/docs/getting-started/](https://www.serverless.com/framework/docs/getting-started/)

## Installation Procedure

1. Install [NodeJS](https://nodejs.org/en/)
2. Install the [Serverless Framework](https://www.serverless.com/framework/docs/getting-started/) and configure it with your AWS instance.
3. Click [HERE](https://bitbucket.org/northwesternitartsdg/dhn2/downloads/DHN2_RC1.zip) to download DH/N2.
4. Unzip "DHN2_<version>.zip" into your preferred directory.
5. Open a terminal or console and change to the directory where the files were un-zipped.
6. Run the following command in your terminal or console and follow the prompts to install Discussion Hero to your AWS instance. Refer to the important notes below regarding information to be input in the prompts.

```shell_session
$ bash scripts/install.sh
```

### Important Notes:

* Choosing an **AWS Region** can affect performance of your application. Follow [this guide](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/RegionsAndAZs.html) to determine which region you'd like to deploy DH/N2.
* Amazon's [Key Management Service (KMS)](https://aws.amazon.com/kms/) is used to encrypt your shared secret and Canvas Developer Tokens.
* You can use an existing **KMS key** if you wish, simply enter "no" at the prompt of "Do you want to generate a **KMS key** in your AWS instance for use in DH?". You will then be prompted to enter the [KMS key ARN](https://docs.aws.amazon.com/kms/latest/developerguide/find-cmk-id-arn.html) you wish to use.
* When choosing a **shared secret**, treat this as a very secure password. Try a long string of letters, numbers, uppercase characters, etc.

## About the DH/N2 Team

Discussion Hero and Nebula 2 are jointly developed by Teaching and Learning Technologies in Northwestern IT Services & Support and The School of Professional Studies at [Northwestern](https://northwestern.edu). Creators of this project are Jacob Guerra-Martinez and David Noffs. All software was developed by Jacob Collins. All avatars were designed by Diana Hernandez. Discussion Hero Logos were designed by Patty Chrastka. Documentation was written by Rachel Goc. Special thanks to Dan Murphy, Reba-Anna Lee, Victoria Getis, Erin Green, Reggie Jackson, Jonathan Diehl, Krissy Wilson, Alita Kendrick, and Suzanne Rovani.