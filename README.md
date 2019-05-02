# AZURE DEVELOPER SERIES - .NET LEGACY APP MIGRATION TO AZURE


## Abstract and Learning Objectives

This workshop enables anyone to **learn, understand and build a Proof of Concept**, in performing a **multi-tiered legacy ASP.NET web application** using Microsoft SQL Server database, platform migration to Azure public cloud, leveraging on **different Azure Platform Azure A Service (PaaS) and Azure Container Services.** 

After an **introductory module** on cloud app migration strategies and patterns, students get introduced to the basics of automating Azure resources deployments using Visual Studio and **Azure Resource Manager (ARM) template**s. Next, attendees will learn about Microsoft SQL database migration to **SQL Azure PaaS**, as well as deploying and migrating **Azure Web Apps**. 
After these foundational platform components, the workshop will totally focus on the core concepts and advantages of using containers for running web apps, based on **Docker, Azure Container Registry (ACR), Azure Container Instance (ACI), as well as how to enable container cloud-scale using Azure Container Services (ACS) with Kubernetes and Azure Kubernetes Service (AKS).**

## Module Overview

The focus of the workshop is having a **Hands-On-Labs experience**, by going through the following exercises and tasks:

•	Deploying a 2-tier Azure Virtual Machine (Webserver and SQL database Server) using ARM-template automation with Visual Studio 2017;

•	Migrating a legacy SQL 2012 database to Azure SQL PaaS (Lift & Shift);

•	Migrating a legacy ASP.NET web application to Azure Web Apps (Lift & Shift); 

•	Containerizing a legacy ASP.NET web application using Docker;

•	Running Azure Container Instance (ACI) from an Azure Container Registry (ACR) image;

•	Deploy and run Azure Container Services (ACS) with Kubernetes;

•	Deploy and run Azure Kubernetes Services (AKS);

•	Managing and Monitoring Azure Container Services (ACS) and Azure Kubernetes Services (AKS);

## Hands-On-Lab Scenario

The baseline of the hands-on-lab scenario is starting from an 8-year-old legacy ASP.NET application, developed around 2010, currently offering a product catalog browsing web page, pulling the product catalog list from a legacy Microsoft SQL Server 2012 database, running on dedicated Windows Server 2012 R2 Virtual Machines. (This could be seen as a subset of a larger application landscape within your organization, think of manufacturing database information, HR solutions, e-commerce platforms,… and alike). Imagine this application is running in our on-premises datacenter, where you want to perform an “application digital migration” to Azure Public cloud. You will use several Azure cloud-native services and solutions, ranging from Virtual Machines, Platform Services and different Container Solutions on Azure.

# Requirements 

## Naming Conventions:
IMPORTANT: Most Azure resources require unique names. Throughout these steps you will see the word “[SUFFIX]” as part of resource names. You should replace this with your initials, guaranteeing those resources get uniquely named.

## Azure Subscription:
Participants need a “pay-as-you-go”, MSDN or other paid Azure subscription
a)	Azure Trial subscriptions won’t work
b)	In one of the Azure Container Services tasks, you are required to create an Azure AD Service Principal, wich typically requires an Azure subscription owner to log in to create this object. If you don’t have the owner right in your Azure subscription, you could ask another person to execute this step for you.
c)	The Azure subscription must allow you to run enough cores, used by the baseline Virtual Machines, but also later on in the tasks when deploying the Azure Container Services, where ACS agent and master machines are getting set up. If you follow the instructions as written out in the lab guide, you need 12 cores. 
d)	If you run this lab setup in your personal or corporate Azure payable subscription, using the configuration as described in the lab guide, the estimated Azure consumption costs for running the setups during the 2 days of the workshop is $20.
Other requirements:
Participants need a local client machine, running a recent Operating System, allowing them to: 
-	browse to https://portal.azure.com from a most-recent browser;
-	establish a secured Remote Desktop (RDP) session to a lab-jumpVM running Windows Server 2016;  

## Alternative Approach:
Where the lab scenario assumes all exercises will be performed from within the lab-jumpVM, (since several tools will be installed on the lab-jumpVM or are already installed by default), participants could also execute (most, if not all…) steps from their local client machine.
The following tools are being used throughout the lab exercises:
-	Visual Studio 2017 community edition (updated to latest version)
-	Docker for Windows (updated to latest version)
-	Azure CLI 2.0 (updated to latest version)
-	Kubernetes CLI (updated to latest version)
Make sure you have these tools installed prior to the workshop, if you are not using the lab-jumpVM. You should also have full administrator rights on your machine to execute certain steps within using these tools.

## Final Remarks:
**VERY IMPORTANT:** You should be typing all of the commands as they appear in the guide, except where explicitly stated in this document. Do not try to copy and paste from Word to your command windows or other documents where you are instructed to enter information shown in this document. There can be issues with Copy and Paste from Word or PDF that result in errors, execution of instructions, or creation of file content.
IMPORTANT: Most Azure resources require unique names. Throughout these steps you will see the word “[SUFFIX]” as part of resource names. You should replace this with your initials, guaranteeing those resources get uniquely named.

Have a great Lab experience!

kind regards, 

Microsoft Azure Developer Series & 007FFFLearning.com teams
