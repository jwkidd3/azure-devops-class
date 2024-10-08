### What is Azure DevOps?

* Implementing DevOps methodology with help of __azure DevOps services__ of __Azure repos__ for __git remote repository management__, __azure pipelines__ for CI/CD , __Azure artifact__ for __artifact's managemnt__ , __Azure test plans__ for __autimation testing__, and __Azure Boards__ for __project managment tool.__

## what is DevOps?
 * Devps of a fusion of Development Dev and operations Ops practices aimed at unifying software development and IT operations. The main goal is the shorten the Development life cycle and provide continous devilvery high software qaulity. DevOps is not a set of tools, it is cultture and mindset promotes most collebartion between development and operations team. This apporach allows more frequent  code release and faster  problem solving and a more agile  responce to market changes.

### Azure DevOps

Azure DevOps is a comprehensive set of development tools and services provided by Microsoft. It offers a complete end-to-end solution for managing the entire application lifecycle, from planning and coding to testing and deployment. Azure DevOps includes the following main components:

- **Azure Boards**: Enables agile planning, tracking work items, and managing backlogs.
- **Azure Repos**: Provides version control and Git repositories for source code management.
- **Azure Pipelines**: Offers robust continuous integration and continuous delivery (CI/CD) capabilities.
- **Azure Test Plans**: Facilitates manual and exploratory testing, test case management, and reporting.
- **Azure Artifacts**: Provides package management for storing and sharing artifacts like libraries and dependencies.

With Azure DevOps, teams can collaborate effectively, automate workflows, and streamline the software development process.

### Differnce between DevOps and Azure DevOps Oand AWS DevOps and GCP DevOps?

*  The main difference between all these, usage of __tools__ change to implement _DevOps methodology__. 

| tools           | DevOps | AWS DevOps | Azure DevOps | GCP DevOps |
| :---------------- | :------ | :----   | :----------- | :---------- |
| git remote repositiry      | Github/Bitbucket/GitLab |  AWS code commit   | Azure Repos| cloud source |
| CI/CD          |   Jenkins/GitLab/ any tools   | code build, code deploy | Azure pipleine | GCP cloud build | 
| configuration management tools  |  Ansible/Chef/any other tools  | Ansible/chef/any other tools | Ansible/chef/ any other tools | Ansible/chef/any other tools |
| Artifact management | Nexus/Jfrog | AWS artifact | Azure artifact | GCP artfifact registery |
| project manament tools| any project tools | any project tools | Azure Boards | any project tools |
| containerzation | Docker | Docker | Docker | Docker | Docker |
| Container orchestation | Kubernetes | Kubernetes , note: creeate kubernetes cluster use "AWS EKS " service | Kubernetes  note: creeate kubernetes cluster use "Azure AKS" service | Kubernetes  note: creeate kubernetes cluster use "GCP GKE" service |
| Infra as a code | terraform | terraform/AWS cloud formation | terraform/Azure ARM templates | Terraform |


* Notes:
  * In the case of __AWS DevOps services__  AWS code commit, AWS code build, AWS code pipline, AWS code deploy and AWS artifact service --> these are part of AWS cloud only.
  * In the case of __AZure DevOps services__  Azure Repo, Azure pipleine, Azure Artifact , Azure test plans, and Azure Boards --> these are seperated from Azure cloud, providing as another product of Microsoft.
     * https://portal.azure.com  --> to connect to Azure cloud
     * https://dev.azure.com/organization-name ---> to connect Azure DevOps services.

  * In the case of __GCP DevOps services__  GCP cloud source, GCP cloud Build, GCP artifact repository --> these are part of __GCP__ cloud only.


### Why Azure DevOps is more popular compare to AWS DevOps?

* Rich matured service compare to AWS DevOps and GCP DevOps.
* No need to develop __custom scripts__ to implement CI/CD.
* pre-defined tasks are avaiable in Azure DevOps for any CI/CD operations.
* to implement and Easy maintain the DevOps operations.

