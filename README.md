# test-lib-demo

![](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white&style=flat)
![](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white&style=flat)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

Demo spring boot application that consumes tes-lib.jar published in public GitHub package at [https://maven.pkg.github.com/dmadunic/test-lib](https://maven.pkg.github.com/dmadunic/test-lib).

# Usage

To build this 


# CI/CD

This project also contains is a simple github action script, **ci.yml**, that performs the following steps:
- checkout
- run tests
- build spring boot jar

For this script to work it requiers for a secret named GH_ACCESS_TOKEN to be created. This secret should contain the value of Personal access token (PATH) with granted access to Public repositores.
