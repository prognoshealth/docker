# Supported tags and respective Dockerfile links

**(reverse order)**

`latest` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/master/circleci_terraform/golang/Dockerfile)

`2.0_0.13.4_1.15.2` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.13.4_1.15.2/circleci_terraform/golang/Dockerfile)

`2.0_0.12.24_1.14.2` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/Terraform0.12.24Golang1.14.2/circleci_terraform/golang/Dockerfile)

`2.0_0.12.6_1.11.5` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.12.6_1.11.5/circleci_terraform/golang/Dockerfile)

`2.0_0.11.13_1.11.5` [(circleci_terraform/golang/Dockerfile)](https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.11.13_1.11.5/circleci_terraform/golang/Dockerfile)

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

`circleci_terraform_golang` is Docker image that bundles terraform into circleci's golang image.

## Tag versioning of image

Tag follows `<circleci_version>_<terraform_version>_<go_version>` versioning scheme. For e.g.

**2.0_0.13.4_1.15.2**: CircleCI Version-`2.0`, Terraform Version-`0.13.4` and Go Version-`1.15.2`

## To Start docker instance

```
$ docker run -d -name circleci_terraform_golang circleci_terraform_golang:2.0_0.13.4_1.15.2
```

## Deploy New Version

- Create a new Branch that captures the new versions
- Update Dockerfile as needed for appropriate version changes

```
> docker build -t prognosai/circleci_terraform_golang:2.0_0.13.4_1.15.2 .
> docker push prognosai/circleci_terraform_golang:2.0_0.13.4_1.15.2
```

## See:
`dockerhub` https://hub.docker.com/repository/docker/prognosai/circleci_terraform_golang
