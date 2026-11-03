---
marp: true
---
<!-- headingDivider: 3 -->
<!-- paginate: true -->

# Building with Mistral Models 

## Introduction 

This lesson will cover: 
- Exploring the different Mistral Models 
- Understanding the use-cases and scenarios for each model 
- Exploring code samples that show the unique features of each model. 

## The Mistral Models 

In this lesson, we will explore 3 different Mistral models: 
**Mistral Large**, **Mistral Small** and **Mistral Nemo**. 

Each of these models is available free on [Microsoft Foundry Models](https://ai.azure.com/catalog/models?WT.mc_id=academic-105485-koreyst). The code in this notebook will be using these models to run the code.

> **Note:** GitHub Models is retiring at the end of July 2026. Here are more details on using [Microsoft Foundry Models](https://learn.microsoft.com/azure/ai-foundry/model-inference/overview?WT.mc_id=academic-105485-koreyst) to prototype with AI models. 


## Mistral Large 2 (2407)
Mistral Large 2 is currently the flagship model from Mistral and is designed for enterprise use. 

The model is an upgrade to the original Mistral Large by offering 
-  Larger Context Window - 128k vs 32k 
-  Better performance on Math and Coding Tasks - 76.9% average accuracy vs 60.4% 
-  Increased multilingual performance - languages include: English, French, German, Spanish, Italian, Portuguese, Dutch, Russian, Chinese, Japanese, Korean, Arabic, and Hindi.

---
With these features, Mistral Large excels at 
- *Retrieval Augmented Generation (RAG)* - due to the larger context window
- *Function Calling* - this model has native function calling which allows integration with external tools and APIs. These calls can be made both in parallel or one after another in a sequential order. 
- *Code Generation* - this model excels on Python, Java, TypeScript and C++ generation. 

## Mistral Small 
Mistral Small is another model in the Mistral family of models under the premier/enterprise category. As the name implies, this model is a Small Language Model (SLM). The advantages of using Mistral Small are that it is: 
- Cost Saving compared to Mistral LLMs like Mistral Large and NeMo - 80% price drop
- Low latency - faster response compared to Mistral's LLMs
- Flexible - can be deployed across different environments with less restrictions on required resources. 


Mistral Small is great for: 
- Text based tasks such as summarization, sentiment analysis and translation. 
- Applications where frequent requests are made due to its cost effectiveness 
- Low latency code tasks like review and code suggestions 

## Mistral NeMo

Compared to the other two models discussed in this lesson, Mistral NeMo is the only free model with an Apache2 License. 

It is viewed as an upgrade to the earlier open source LLM from Mistral, Mistral 7B. 

Some other features of the NeMo model are: 

- *More efficient tokenization:* This model uses the Tekken tokenizer over the more commonly used tiktoken. This allows for better performance over more languages and code. 

- *Finetuning:* The base model is available for finetuning. This allows for more flexibility for use-cases where finetuning may be needed. 

- *Native Function Calling* - Like Mistral Large, this model has been trained on function calling. This makes it unique as being one of the first open source models to do so. 
