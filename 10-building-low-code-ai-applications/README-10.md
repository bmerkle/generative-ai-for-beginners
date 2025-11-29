---
marp: true
---
<!-- headingDivider: 3 -->
<!-- paginate: true -->

# Building Low Code AI Applications

Building apps and solutions has become more easier for traditional developers and non-developers through the use of Low Code Development Platforms. Low Code Development Platforms enable you to build apps and solutions with little to no code. 

This lesson covers:

- Introduction to Generative AI in Power Platform
- Introduction to Copilot and how to use it
- Using Generative AI to build apps and flows in Power Platform
- Understanding the AI Models in Power Platform with AI Builder

## Learning Goals

By the end of this lesson, you will be able to:

- Understand how Copilot works in Power Platform.

- Build a Student Assignment Tracker App for our education startup.

- Build an Invoice Processing Flow that uses AI to extract information from invoices.

- Apply best practices when using the Create Text with GPT AI Model.

## The tools and technologies that you will use in this lesson are:

- **Power Apps**, for the Student Assignment Tracker app, which provides a low-code development environment for building apps to track, manage and interact with data.

- **Dataverse**, for storing the data for the Student Assignment Tracker app where Dataverse will provide a low-code data platform for storing the app's data.

- **Power Automate**, for the Invoice Processing flow where you will have low-code development environment for building workflows to automate the Invoice Processing process.

- **AI Builder**, for the Invoice Processing AI Model where you will use prebuilt AI Models to process the invoices for our startup.

## Generative AI in Power Platform

Enhancing low-code development and application with generative AI is a key focus area for Power Platform. The goal is to enable everyone to build AI-powered apps, sites, dashboards and automate processes with AI, _without requiring any data science expertise_. This goal is achieved by integrating generative AI into the low-code development experience in Power Platform in the form of Copilot and AI Builder.

### How does this work?

Copilot is an AI assistant that enables you to build Power Platform solutions by describing your requirements in a series of conversational steps using natural language. You can for example instruct your AI assistant to state what fields your app will use and it will create both the app and the underlying data model or you could specify how to set up a flow in Power Automate.

AI Builder is a low-code AI capability available in Power Platform that enables you to use AI Models to help you to automate processes and predict outcomes. With AI Builder you can bring AI to your apps and flows that connect to your data in Dataverse or in various cloud data sources, such as SharePoint, OneDrive or Azure.


### Copilot in Power Apps

As part of the Power Platform, Power Apps provides a low-code development environment for building apps to track, manage and interact with data. It's a suite of app development services with a scalable data platform and the ability to connect to cloud services and on-premises data. Power Apps allows you to build apps that run on browsers, tablets, and phones, and can be shared with co-workers. Power Apps eases users into app development with a simple interface, so that every business user or pro developer can build custom apps. The app development experience is also enhanced with Generative AI through Copilot.

The copilot AI assistant feature in Power Apps enables you to describe what kind of app you need and what information you want your app to track, collect, or show. Copilot then generates a responsive Canvas app based on your description. You can then customize the app to meet your needs. The AI Copilot also generates and suggests a Dataverse Table with the fields you need to store the data you want to track and some sample data. 

### Copilot in Power Automate

As part of the Power Platform, Power Automate lets users create automated workflows between applications and services. It helps automate repetitive business processes such as communication, data collection, and decision approvals. Its simple interface allows users with every technical competence (from beginners to seasoned developers) to automate work tasks. The workflow development experience is also enhanced with Generative AI through Copilot.

The copilot AI assistant feature in Power Automate enables you to describe what kind of flow you need and what actions you want your flow to perform. Copilot then generates a flow based on your description. You can then customize the flow to meet your needs. The AI Copilot also generates and suggests the actions you need to perform the task you want to automate. We will look at what flows are and how you can use them in Power Automate in this lesson later. You can then customize the actions to meet your needs using the AI Copilot assistant feature through conversational steps. This feature is readily available from the Power Automate home screen.

