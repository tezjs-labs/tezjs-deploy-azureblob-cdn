# Deploy to Azure blob and cdn
In this guide, you will learn how to deploy your tezjs site to Azure Blob and CDN configuration.

## Deployed Url:
https://tezjsblobcdn.azureedge.net/

## Preparing for deployment:
Run the following command to create tezjs project:
  - `npm create tez@latest`
  - `cd [projectName]`
  - `npm install` - for installing the required dependencies
  - `npm run build` - for build the project
  - `npm run dev` - for run the project

## Pre-requisites
Make sure you have:
  - Azure account.
  - Node installed in your machine.

## Deployment
Go to https://www.portal.azure.com/ and login, create team. 

- Create Resource group and Storage account from Azure Portal
- Enable static website option from data management section
- Primary url get like https://tezjsblobcdn.z29.web.core.windows.net/
- Add index.html in Index document name of static website option from data management section
- Upload dist folder content to $web folder
- Select and configure Azure CDN option from Security + networking section
- Create new CDN Profile
- Select Origin hostname as a static web app


