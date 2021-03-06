# How to Contribute ?
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)  
[![husky](https://img.shields.io/badge/husky-v3.0.4-blue)](https://www.npmjs.com/package/husky)
[![commitlint](https://img.shields.io/badge/commitlint-v8.1.0-green)](https://www.npmjs.com/package/commitlint)

This repository accepts contributions via **Merge Requests**.  
This document outlines some of the conventions on development workflow, commit message formatting, contact points and other resources to make it easier to get your contribution accepted.  
We gratefully welcome improvements to documentation as well as to code.  

## Installation

Before installing whiteapp, we recommand you to read this folowing documents :  

- ReactJS whiteapp [readme file](https://apps.bsc.aws.societegenerale.com/gitlab/dex/frontend/react-whiteapp/blob/master/README.md)  

- ReactJS whiteapp [contributing file](https://apps.bsc.aws.societegenerale.com/gitlab/dex/frontend/react-whiteapp/blob/master/CONTRIBUTING.md)  

- Configure [proxy](https://sgithub.fr.world.socgen/bsc/docker-for-windows#configure-docker-proxy) and [NPM](https://apps.bsc.aws.societegenerale.com/gitlab/dex/frontend/react-whiteapp/blob/develop/README.md#installation)

- [DEX documentations](https://apps.bsc.aws.societegenerale.com/gitlab/dex/welcome)  


### Prerequisite

- [![node](https://img.shields.io/badge/node-v10.16.0-blue)](https://apps.bsc.aws.societegenerale.com/gitlab/dex/backend/nestjs-api-whiteapp/commits/develop)  

- :information_source: see [this section](https://sgithub.fr.world.socgen/bsc/docker-for-windows#configure-docker-proxy)

#### Procedure  

##### How to

###### Read SG Connect core module documentation:
:information_source: [nestjs-sg-connect](https://sgithub.fr.world.socgen/nestjs/sg-nestjs/blob/master/@sg-nestjs/nestjs-sg-connect/README.md)

###### Read Swagger UI core module documentation:
:information_source: [nestjs-swagger-ui](https://sgithub.fr.world.socgen/nestjs/sg-nestjs/blob/master/%40sg-nestjs/nestjs-swagger-ui/README.md)


#### Usage

##### Development environment :

:link: Open http://localhost:9999/api/v1/employees

##### Swagger page for developpement :

:link: Open http://localhost:9999/swagger/#/

## Making a change

[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)  

Before making any significant changes, **[please open an issue](https://apps.bsc.aws.societegenerale.com/gitlab/dex/backend/nestjs-api-whiteapp/issues)**. Discussing your proposed changes ahead of time will make the contribution process smooth for everyone.  

We have 2 protected branches: `master` & `develop`  

- Create your bugfix or feature branch from develop ([Git flow](https://danielkummer.github.io/git-flow-cheatsheet/index.html))  

- Code your bugfix or your feature  

- Includes tests for new functionality.  

- Ensure your code pass tests by running `npm run test`  

- Ensure your code respect our linter rules `npm run lint`  

- Ensure your code build well `npm run build`  

- Has [a good commit](https://chris.beams.io/posts/git-commit/) message:

    - Follow [conventional commit format](https://www.conventionalcommits.org/en/v1.0.0-beta.4/). 
    - Separate subject from body with a blank line
    - Limit the subject line to 70 characters
    - Do not end the subject line with a period
    - Use the imperative mood in the subject line
    - Wrap the body at 72 characters
    - Use the body to explain what and why instead of how  

- Create a merge request to develop branch  

- Once your merge request is approved by maintainers, your branch is merged to develop

**Maintainers merge `develop` branch to `master` branch

`semantic-release` will automatically create a tag and generate the changelog based on the commit message.
