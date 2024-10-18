## 🚀 About Me
I'm a junior DevOps engineer with some expertise in BackEnd development using Java and Node.js; scripting skills with Python, Bash and JavaScript; besides CI/CD and cloud knowledge of AWS and Azure DevOps tools ...

![Logo](https://e1.pxfuel.com/desktop-wallpaper/541/577/desktop-wallpaper-fantastic-backgrounds.jpg)
![linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![javascript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![nodejs](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![mysql](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white)
![aws](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![azuredevops](https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azure-devops&logoColor=white)

## 🔗 Portfolio
[![portfolio](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RecursiveDeveloper)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jhoan-jesus-ortiz-sandoval-a66152198/)

# Serverless calculator

Build and operate your own CI/CD serverless application using Azure DevOps as your deployment tool, Snyk as your SCA scanner and AWS as your cloud target to use Lambda and API Gateway to serve a serverless calculator static web page.

![image](https://raw.githubusercontent.com/RecursiveDeveloper/static-media-content/refs/heads/main/Serverless_Calculator.png)

## Tech Stack 

- **Client:** API Gateway
- **Server:** Lambda, Nodejs
- **Database:** ---
- **Cloud provider:** AWS
- **Tools:** Azure DevOps, Snyk

## Installation

1. Set up an [Azure DevOps project](https://learn.microsoft.com/en-us/azure/devops/organizations/projects/create-project?view=azure-devops&tabs=browser)
2. Use GitHub as your source pipeline and code configuration [GitHub Repository with Azure DevOps Pipelines](https://spr.com/using-github-repository-with-azure-devops-pipelines/)
3. Create a Snyk account for SCA scanning [Create or log in to a Snyk account](https://docs.snyk.io/getting-started#create-or-log-in-to-a-snyk-account)
4. Add Snyk extension to your Azure DevOps project [Install the Snyk extension](https://docs.snyk.io/scm-ide-and-ci-cd-integrations/snyk-ci-cd-integrations/azure-pipelines-integration/install-the-snyk-extension-for-your-azure-pipelines) as well as AWS Toolkit extension [AWS Toolkit](https://docs.aws.amazon.com/vsts/latest/userguide/getting-started.html#install-the-aws-tools-for-vsts-extension)
5. Create a service connection in your Azure DevOps project linked to AWS and name it as **AWS_Connection** [Create a service connection](https://learn.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops#create-a-service-connection)
6. Create a service connection in your Azure DevOps project linked to your Snyk account and name it as **Snyk_Scanner** [Snyk service connection](https://docs.snyk.io/scm-ide-and-ci-cd-integrations/snyk-ci-cd-integrations/azure-pipelines-integration/install-the-snyk-extension-for-your-azure-pipelines#step-for-installing-the-snyk-extension-for-azure-pipelines) 
7. Create an AWS Lambda Function and change **index.handler** configuration to **lambda.handler** [Create your first Lambda function](https://docs.aws.amazon.com/lambda/latest/dg/getting-started.html)
8. (optional) Create an Amazon API Gateway Rest API [Create a REST API with a Lambda proxy integration](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-create-api-as-simple-proxy-for-lambda.html). 
    * Leave resource as default (/) and set up an **Any** method within this resource.
    * Deploy your API creating a new stage named **calculator**
    * Invoke URL should look like this https://xxxxx.execute-api.xx-xxxx-x.amazonaws.com/calculator


## Deployment

To deploy this project, get into your Azure DevOps project and run Azure DevOps pipeline manually. Or make any change to app folder inside this project to trigger pipeline execution automatically.

For more informations about Azure DevOps pipelines check [Azure Pipelines documentation](https://learn.microsoft.com/en-us/azure/devops/pipelines/?view=azure-devops)

## Authors

- [@RecursiveDeveloper](https://github.com/RecursiveDeveloper)
- Based on [@burak-aws](https://github.com/aws-samples/aws-lambda-demo-with-node-express)

## License

[MIT](https://choosealicense.com/licenses/mit/)
