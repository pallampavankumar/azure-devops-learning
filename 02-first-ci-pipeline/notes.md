# DevOps Core Concepts

## Pipeline
A pipeline is an automated process that builds, tests, and deploys an application.

Example flow:
Code → Build → Test → Deploy

---

## Agent
An agent is a machine that runs the pipeline.

It:
- Downloads the code
- Executes build commands
- Runs tests
- Deploys the application

### Types of agents
1. Microsoft-hosted agent
   - Provided by Azure
   - Managed automatically
2. Self-hosted agent
   - Your own machine or server

---

## Parallel Job
A parallel job is the number of pipelines that can run at the same time.

Example:
- 1 parallel job → only one pipeline at a time
- 2 parallel jobs → two pipelines at the same time

---

## Free Build Minutes
When using Microsoft-hosted agents, Azure gives a limited number of free build minutes per month.

Example:
- 1 parallel job
- 1800 minutes per month

New organizations must request this free quota.

---

## Service Connection
A service connection allows Azure DevOps to access external services.

Example:
- Azure subscription
- Docker registry
- GitHub

It is used by pipelines to deploy resources.
