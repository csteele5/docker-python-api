# docker-python-api
CFProject1 - 1) Containerized python program accessible via API

## Overview

This repo is a cloud formation deployment of a python api application in an EC2 + RDS stack.  There is currently no release pipeline or automated deployment. The goal is to use a YAML file to manually build a stack, then define an application and deploy it to that stack.  In variation one of this repo, the stack will be an EC2 instance, which will run a docker image with no database. The deployments will be executed via CLI commands.

## Build Outline

- Create a new git repo with readme
- Create AWS KeyPair for SSH access to EC2 instance
- Configure AWS CLI
- Define stack in YAML - containing EC2 instance
- Update stack definition to install docker on EC2 instance
- Update stack to add RDS for MySQL database
- Define Docker Compose for application deployment
- Deploy the application using docker compose & test

## References

Cloudformation tutorial: https://www.youtube.com/watch?v=8J0g_xWUzV0
Docker/Python/API tutorial: https://www.youtube.com/watch?v=4T5Gnrmzjak

## Development Team

| Name | Developer Handle | Email | Role |
|------|------------------|-------|------|
| Charles Steele | @csteele5 | siegcw@yahoo.com | Domain Architect |
| Charles Steele | @csteele5 | siegcw@yahoo.com | Lead Engineer |
| Charles Steele | @csteele5 | siegcw@yahoo.com | API Designer and Developer |
