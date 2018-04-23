# Supported tags and respective Dockerfile links

`latest` [(terraform_kitchen_awspec/Dockerfile)](https://github.com/medivo/Docker/blob/master/terraform_kitchen_awspec/Dockerfile)

`0.11.7` [(terraform_kitchen_awspec/Dockerfile)](https://github.com/medivo/Docker/blob/terraform_0.11.7/terraform_kitchen_awspec/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/medivo/Docker/issues
    
- **Maintained by:**

    Prognos.ai, sectechops@prognos.ai

- **Supported architectures:**

    amd64

# What is terraform_kitchen_awspec?

`terraform_kitchen_awspec` is Docker image that contains Terraform, Kitchen and awspec installed in docker image.

## Image includes following packages

- Terraform: 0.11.7
- Kitchen.ci
- Awspec
- Ruby 2.4.3
- kitchen-vagrant gem
- kitchen-ansible gem
- kitchen-inspec gem
- kitchen-terraform gem
- kitchen-verifier-awspec gem
- rspec_junit_formatter

## To Start docker instance

```
$ docker run -d -name terraform_kitchen terraform_kitchen_awspec:0.111.7
```
