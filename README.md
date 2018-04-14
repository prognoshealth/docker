# Supported tags and respective Dockerfile links

    `2.12.5_2.3.0_1.1.2`, `latest` [(scala_spark_sbt/Dockerfile)](https://github.com/medivo/Docker/blob/master/scala_spark_sbt/Dockerfile)
    `2.11.12_2.3.0_0.13.17` [(scala_spark_sbt/Dockerfile)](https://github.com/medivo/Docker/blob/master/scala_spark_sbt/Dockerfile)

# Quick Reference
- **Where to file issues:**

    https://github.com/medivo/Docker/issues
    
- **Maintained by:**

    Prognos.ai, sectechops@prognos.ai

- **Supported architectures:**

    amd64

# What is scala_spark_sbt?

    `scala_spark_sbt` is Docker image that contains Scala, Spark and SBT installed in docker image.

## Tag versioning of image

    Tag follows `<scala_version>_<spark_version>_<sbt_version>` versioning scheme.
    For e.g.
    **2.11.12_2.3.0_0.13.17**: Scala Version-`2.11.12`, Spark Version-`2.3.0` and SBT Version-`0.13.17`

## To Start docker instance
    ```
    $ docker run -d -name scala_spark scala_spark_sbt:2.11.12_2.3.0_0.13.17
    ```


    

