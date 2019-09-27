# Supported tags and respective Dockerfile links

`2.0_0.12.7_1.13.1_11.0.4.` [Dockerfile]((https://github.com/prognoshealth/docker/blob/circleci_terraform_golang_2.0_0.12.6_1.11.5/circleci_terraform/golang/Dockerfile))


# Quick Reference
- **Where to file issues:**

    https://github.com/prognoshealth/docker/issues
    
- **Maintained by:**

    Prognos.ai, developers+otters@prognos.ai

- **Supported architectures:**

    amd64

# What is circleci_terraform_golang?

`circleci_terraform_goloang_with_java` is Docker image that contains bundles terraform into circleci's golang image and installs the most recent version of the jre for debian.

## Tag versioning of image

Tag follows `<circleci_version>_<terraform_version>_<go_version>_<java_version>` versioning scheme. 
example:

**2.0_1.12.7_1.13.1_11.0.4**: CircleCI Version-`2.0`, Terraform Version-`0.12.7` and Go Version-`1.12.9` and Java Version `11.0.4`

## To Start docker instance
example:
```
$ docker run -d prognosai/circleci_terraform_goloang_with_java:2.0_0.12.7_1.12.9
```

docker run -it prognosai/circleci_terraform_goloang_with_java:2.0_0.12.7_1.12.9 bash

## Deploy New Version

- Create a new Branch that captures the new versions
- Update Dockerfile as needed for appropriate version changes

example:
```
> docker build -t prognosai/circleci_terraform_goloang_with_java:2.0_0.12.7_1.12.9 . 
> docker push prognosai/circleci_terraform_goloang_with_java:2.0_0.12.7_1.12.9
```