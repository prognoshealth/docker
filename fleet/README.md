# Supported tags and respective Dockerfile links

`latest` [(fleet/Dockerfile)](https://github.com/prognoshealth/docker/blob/master/fleet/Dockerfile)

`2.0.0-rc3` [(fleet_2_0_0_rc3/Dockerfile)](https://github.com/prognoshealth/docker/blob/fleet_2_0_0_rc3/fleet/Dockerfile)

`2.0.0` [(fleet/Dockerfile)](https://github.com/prognoshealth/docker/blob/fleet_2_0_0/fleet/Dockerfile)

`2.0.2` [(fleet/Dockerfile)](https://github.com/prognoshealth/docker/blob/fleet_2_0_2/fleet/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/prognoshealth/docker/issues
    
- **Maintained by:**

    Prognos.ai, sectechops@prognos.ai

- **Supported architectures:**

    amd64

# What is fleet?

`fleet` is Docker image that contains Kolide Fleet and Cloudwatch log agent configured.

## To Start docker instance

```
$ docker run -d -name fleet fleet:2.0.0
```
