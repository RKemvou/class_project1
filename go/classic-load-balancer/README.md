# Classic Load Balancer
<!--BEGIN STABILITY BANNER-->
---

![Stability: Stable](https://img.shields.io/badge/stability-Stable-success.svg?style=for-the-badge)

> **This is a stable example. It should successfully build out of the box**
>
> This examples is built on Construct Libraries marked "Stable" and does not have any infrastructure prerequisites to build.

---
<!--END STABILITY BANNER-->

**NOTICE**: Go support is still in Developer Preview. This implies that APIs may
change while we address early feedback from the community. We would love to hear
about your experience through GitHub issues.

This example creates an AutoScalingGroup (containing a Micro-T2 EC2 machine running the Amazon Linux AMI), and a ClassicLoadBalancer inside a shared VPC. It hooks up an open listener from the Load Balancer to the Scaling Group to indicate how many targets to balance between.

For more info on using Auto Scaling with Load Balancing see the AutoScaling guide [here](https://docs.aws.amazon.com/autoscaling/ec2/userguide/autoscaling-load-balancer.html).

## Deploy

Run `cdk deploy`. This will deploy / redeploy your Stack to your AWS Account.

After the deployment you will see the API's URL, which represents the url you can then use.

## Synthesize Cloudformation Template

To see the Cloudformation template generated by the CDK, run `cdk synth`, then check the output file in the "cdk.out" directory.
