# Supported tags and respective Dockerfile links

`latest` [(fleet/Dockerfile)](https://github.com/medivo/Docker/blob/master/fleet/Dockerfile)

`2.0.0-rc3` [(fleet_2_0_0_rc3/Dockerfile)](https://github.com/medivo/Docker/blob/fleet_2_0_0_rc3/fleet/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/medivo/Docker/issues
    
- **Maintained by:**

    Prognos.ai, sectechops@prognos.ai

- **Supported architectures:**

    amd64

# What is fleet?

`fleet` is Docker image that contains Kolide Fleet and Cloudwatch log agent configured.

## To Start docker instance

```
$ docker run -d -name fleet fleet:2.0.0-rc3
```