# GitHub Actions CI/CD with Azure Cloud Platform

A hands-on learning repository for mastering **GitHub Actions**, **CI/CD automation**, and production-ready workflow design through practical examples.

---

## Objectives

- Understand GitHub Actions from scratch
- Learn how CI/CD works in modern software development
- Build reusable GitHub workflows
- Automate testing, building, and deployment
- Learn workflow orchestration using multiple jobs
- Prepare for production-grade DevOps pipelines


# Prerequisites

Before starting this lab, you should have:

- Basic Git & GitHub knowledge
- Basic Linux terminal commands
- Basic YAML syntax
- Familiarity with any programming language
- Basic understanding of Docker (recommended)


# Learning Roadmap

## Introduction

- What is GitHub Actions?
- Why Automation Matters
- Manual vs Automated Deployment
- Daily Software Development Workflow
- GitHub Actions Overview


## CI/CD Fundamentals

- What is Continuous Integration (CI)
- What is Continuous Deployment (CD)
- Manual Deployment Process
- Automated Deployment Process
- Benefits of CI/CD


## GitHub Actions Architecture

Learn how GitHub Actions works internally.

Topics

- Repository Events
- Workflow
- Runner
- Job
- Step
- Action
- YAML Configuration


## First Workflow

Create your first GitHub Actions workflow.

Topics

- `.github/workflows`
- YAML file
- Workflow name
- Runner
- Steps
- Execute shell commands

Example

```yaml
name: First Workflow
```


## Workflow Events

Trigger workflows using different events.

Topics

### Push Event

```yaml
on:
  push:
```


### Manual Workflow

```yaml
workflow_dispatch
```


### Branch Specific Workflow

```yaml
on:
  push:
    branches:
      - main
```


### Scheduled Workflow

Cron Jobs

```yaml
schedule:
```


## Runners

Understand where workflows execute.

Topics

- ubuntu-latest
- windows-latest
- macos-latest
- GitHub Hosted Runner
- Self Hosted Runner


## Jobs

Understand workflow jobs.

Topics

- Single Job
- Multiple Jobs
- Parallel Jobs

Example

```yaml
jobs:
```


## Job Dependencies

Execute jobs sequentially.

Topics

- needs keyword
- Job Dependency Graph
- Sequential Execution

Example

```yaml
needs:
  - build
```


## Conditional Workflows

Execute workflows only when specific files change.

Topics

- paths
- paths-ignore
- Conditional execution

Example

```yaml
paths:
  - backend/**
```


## Passing Inputs

Topics

- workflow_dispatch inputs
- Required inputs
- Default values

Example

```yaml
workflow_dispatch:
```


## Passing Values Between Jobs

Topics

- Outputs
- GitHub Output
- Job Outputs
- Context


## Reusable Workflows

Topics

- workflow_call
- Workflow reuse
- Sharing workflows


## Composite Actions

Topics

- Composite Action
- Action.yml
- Reusable commands


## Real CI/CD Example

Pipeline Example

```
Developer
     │
     ▼
git push
     │
     ▼
GitHub Actions
     │
     ├── Checkout
     ├── Install Dependencies
     ├── Run Tests
     ├── Build Docker Image
     ├── Push Image
     └── Deploy
```


# Repository Structure

```
.github/
└── workflows/
    ├── first-workflow.yml
    ├── manual-workflow.yml
    ├── cron-workflow.yml
    ├── multi-job.yml
    ├── dependency-job.yml
    ├── conditional.yml
    ├── reusable.yml
    └── composite.yml

examples/

docs/

README.md
```


# Concepts Covered

- GitHub Actions
- CI
- CD
- Workflow
- Events
- Jobs
- Steps
- Runners
- GitHub Hosted Runner
- Self Hosted Runner
- YAML
- Workflow Dispatch
- Push Event
- Cron Schedule
- Job Dependencies
- Conditional Workflow
- Workflow Inputs
- Outputs
- Reusable Workflow
- Composite Action


# Learning Outcome


- Design professional GitHub Actions workflows
- Automate software delivery
- Build CI pipelines
- Build CD pipelines
- Use reusable workflows
- Build production-ready automation pipelines
- Understand enterprise GitHub Actions architecture


## Later

- Docker CI/CD
- Azure VM Deployment
- AWS EC2 Deployment
- Azure Container Registry (ACR)
- Amazon ECR
- Nginx Deployment
- Self Hosted Runner
- Kubernetes Deployment
- Terraform Automation
- Pulumi Automation