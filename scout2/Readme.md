# Supported tags and respective Dockerfile links

`latest` [(scout2/Dockerfile)](https://github.com/medivo/Docker/blob/master/scout2/Dockerfile)
`3.2.0` [(scout2/Dockerfile)](https://github.com/medivo/Docker/blob/master/scout2/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/medivo/Docker/issues

- **Maintained by:**

    Prognos.ai, sectechops@prognos.ai

- **Supported architectures:**

    amd64

# What is scout2?

`scout2` is Docker image that contains awsscout2 installed which one of the tool for auditing the security of an AWS account.

## To Start docker instance

```
$ docker run -it -e AWS_ACCESS_KEY_ID=${AWS_ACCESS_KEY_ID} -e AWS_SECRET_ACCESS_KEY=${AWS_SECRET_ACCESS_KEY}  scout2
```
