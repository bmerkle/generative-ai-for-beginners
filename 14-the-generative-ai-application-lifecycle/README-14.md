---
marp: true
---
<!-- headingDivider: 3 -->
<!-- paginate: true -->

## Introduction

In this chapter, you will:

- Understand the Paradigm Shift from MLOps to LLMOps
- The LLM Lifecycle
- Lifecycle Tooling
- Lifecycle Metrification and Evaluation

## Understand the Paradigm Shift from MLOps to LLMOps

LLMs are a new tool in the Artificial Intelligence arsenal, they are incredibly powerful in analysis and generation tasks for applications, however this power has some consequences in how we streamline AI and Classic Machine Learning tasks.

With this, we need a new Paradigm to adapt this tool in a dynamic, with the correct incentives. We can categorize older AI apps as "ML Apps" and newer AI Apps as "GenAI Apps" or just "AI Apps", reflecting the mainstream technology and techniques used at the time. This shifts our narrative in multiple ways, look at the following comparison.

---
![LLMOps vs. MLOps comparison](./images/01-llmops-shift.png?WT.mc_id=academic-105485-koreys)

---
Notice that in LLMOps, we are more focused on the App Developers, using integrations as a key point, using "Models-as-a-Service" and thinking in the following points for metrics.

- Quality: Response quality
- Harm: Responsible AI
- Honesty: Response groundedness (Makes sense? It is correct?)
- Cost: Solution Budget
- Latency: Avg. time for token response

## The LLM Lifecycle


![LLMOps infographic](./images/02-llmops.png?WT.mc_id=academic-105485-koreys)

---
![LLMOps Workflow](./images/03-llm-stage-flows.png?WT.mc_id=academic-105485-koreys)

## Lifecycle Tooling

For Tooling, Microsoft provides the [Azure AI Platform](https://azure.microsoft.com/solutions/ai/?WT.mc_id=academic-105485-koreys) and [PromptFlow](https://microsoft.github.io/promptflow/index.html?WT.mc_id=academic-105485-koreyst) facilitate and make your cycle easy to implement and ready to go.

---
The [Azure AI Platform](https://azure.microsoft.com/solutions/ai/?WT.mc_id=academic-105485-koreys), allows you to use [AI Studio](https://ai.azure.com/?WT.mc_id=academic-105485-koreys). AI Studio is a web portal allows you to Explore models, samples and tools. Managing your resources, UI development flows and SDK/CLI options for Code-First development.

---
![Azure AI possibilities](./images/04-azure-ai-platform.png?WT.mc_id=academic-105485-koreys)

Azure AI, allows you to use multiple resources, to manage your operations, services, projects, vector search and databases needs.

---
![LLMOps with Azure AI](./images/05-llm-azure-ai-prompt.png?WT.mc_id=academic-105485-koreys)

Construct, from Proof-of-Concept(POC) until large scale applications with PromptFlow:

- Design and Build apps from VS Code, with visual and functional tools
- Test and fine-tune your apps for quality AI, with ease.
- Use Azure AI Studio to Integrate and Iterate with cloud, Push and Deploy for quick integration.

---
![LLMOps with PromptFlow](./images/06-llm-promptflow.png?WT.mc_id=academic-105485-koreys)

