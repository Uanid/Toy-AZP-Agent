# Lightweight Azure Pipeline Agent

Original Dockerfile from [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops)

## How to use

In Docker Compose
```
version: "3.7"
services:
  agent:
    image: uanid/lightweight-azure-pipeline-agent:latest
    environment:
      AZP_URL: https://dev.azure.com/<enter-your-organization>
      AZP_TOKEN: <enter-your-access-token>
      AZP_POOL: <enter-your-agent-pool>
    privileged: true
```

