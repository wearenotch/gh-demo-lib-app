# gh-demo-lib-app

[![CI Build](https://github.com/ag04/gh-demo-lib-app/actions/workflows/ci.yml/badge.svg)](https://github.com/dmadunic/test-lib-demo/actions/workflows/ci.yml)
![](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white&style=flat)
![](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white&style=flat)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

Demo spring boot application that consumes gh-demo-lib.jar published in public GitHub package at [https://maven.pkg.github.com/ag04/gh-demo-lib](https://maven.pkg.github.com/ag04/gh-demo-lib).

# Usage

To build this app localy, you need to create file named `.env` in the root folder with the following content:
```
gh_username=your_github_usernam
gh_token=value_of_your_personall_access_token_with_access_to_public_repositories
```

Once this is done project can be built by running:
```bash
./gradlew clean bootJar
```

# CI/CD

This project also contains a simple github action script, **ci.yml**, that performs the following steps:
- checkout
- run tests
- build spring boot jar

For this script to work it requiers for a secret named GH_ACCESS_TOKEN to be created. This secret should contain the value of Personal access token (PATH) with granted access to Public repositores.
