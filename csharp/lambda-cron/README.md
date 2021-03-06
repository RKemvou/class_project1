
# Lambda Cron
<!--BEGIN STABILITY BANNER-->
---

![Stability: Stable](https://img.shields.io/badge/stability-Stable-success.svg?style=for-the-badge)

> **This is a stable example. It should successfully build out of the box**
>
> This examples is built on Construct Libraries marked "Stable" and does not have any infrastructure
prerequisites to build.

---
<!--END STABILITY BANNER-->

This example creates a new lambda function that executes every day at 6pm UTC, as dictated by a cron
scheduled event.

## Build

To build this app, you need to be in this example's root folder. Then run the following:

```bash
npm install -g aws-cdk
dotnet build src
```

This will install the necessary CDK, then this example's dependencies, and then build your .Net
Project files and your CloudFormation template.

## Test

To test this app after it is built, you need to be in the `LambdaCron.Tests` folder. Then you can
call `dotnet test` to run the test suite that uses the XUnit along with the CDK
[Assertions](https://docs.aws.amazon.com/cdk/api/latest/dotnet/api/Amazon.CDK.Assertions.html)
library. Assuming you are in the root folder:

```bash
cd src/LambdaCron.Tests
dotnet test
```

## Deploy

Run `cdk deploy LambdaCronStack`. This will deploy / redeploy your Stack to your AWS Account.

After the deployment you will see the API's URL, which represents the url you can then use.

## Synthesize Cloudformation Template

To see the Cloudformation template generated by the CDK, run `cdk synth LambdaCronStack`, then check
the output file in the"cdk.out" directory.