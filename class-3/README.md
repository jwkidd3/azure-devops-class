## azure devop yaml strcutre


![azure-yaml-strcutre](./images/piplene-strcutre.svg)
* https://learn.microsoft.com/en-us/azure/devops/pipelines/yaml-schema/?view=azure-pipelines


```
trigger:
- master
- develop
- feature/*

pool:
  vmImage: ubuntu-latest
```

```
trigger:
- master
- develop
- feature/*

pool:
  vmImage: ubuntu-latest

steps:
- script: |
    echo "bala"
    echo "bhaskar"
```

* Build across multiple platforms
```
* https://learn.microsoft.com/en-us/azure/devops/pipelines/customize-pipeline?view=azure-devops

trigger:
- main

strategy:
  matrix:
    linux:
      imageName: "ubuntu-latest"
    mac:
      imageName: "macOS-latest"
    windows:
      imageName: "windows-latest"
  maxParallel: 1

pool:
  vmImage: $(imageName)

steps:
- script: 'dotnet --info'
  displayName: 'Command Line Script'
```

* Extends
  * Extends a pipeline using a template.

```
trigger:
- main


pool:
  vmImage: "ubuntu-latest"


extends:
  template: CommonTemplate.yml

- script: 'dotnet --info'
  displayName: 'Command Line Script'
```


* JOBS

*  create differnet jobs in the pipeline

```
jobs:
- job: MyJob
  displayName: My First Job
  continueOnError: true
  workspace:
    clean: outputs
  steps:
  - script: echo My first job
```