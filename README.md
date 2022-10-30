# stopadforms-infra

Infrastructure for deploying stopadforms as a containerized application to AWS


[Bootstrap](https://docs.aws.amazon.com/cdk/v2/guide/bootstrapping.html) CDK in the AWS account.

Edit `.github/workflows/docker_deploy.yml`, setting the parameters listed under `env`, including the choice of container (and version) to deploy.

Edit `cdk/docker_fargate/docker_fargate_stack.py` as desired to set parameters like number of containers, CPU, memory, and to set up auto-scaling.

Push the changes to GitHub'. This will initiate the workflow and deploy the application.
