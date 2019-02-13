# Supported tags and respective Dockerfile links

`latest` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/master/circleci_terraform/golang/Dockerfile)

`2.0_0.11.11_1.11.5` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.11.11_1.11.5/circleci_terraform/golang/Dockerfile)

`2.0_0.11.11_1.10` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.11.11_1.10/circleci_terraform/golang/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/prognoshealth/docker/issues
    
- **Maintained by:**

    Prognos.ai, developers+sponges@prognos.ai

- **Supported architectures:**

    amd64

# What is circleci_terraform_golang?

`circleci_terraform_golang` is Docker image that contains bundles terraform into circleci's golang image.

## Tag versioning of image

Tag follows `<circleci_version>_<terraform_version>_<go_version>` versioning scheme. For e.g.

**2.0_0.11.11_1.10**: CircleCI Version-`2.0`, Terraform Version-`0.11.11` and Go Version-`1.10`

## To Start docker instance

```
$ docker run -d -name circleci_terraform_golang circleci_terraform_golang:2.0_0.11.11_1.10
```
