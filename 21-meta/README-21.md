---
marp: true
---
<!-- headingDivider: 3 -->
<!-- paginate: true -->

# Building With the Meta Family Models 

## Introduction 

This lesson will cover: 

- Exploring the two main Meta family models - Llama 3.1 and Llama 3.2, plus the currently available alternatives used in the code samples (Llama 3.3 and Llama 4) 
- Understanding the use-cases and scenarios for each model 
- Code sample to show the unique features of each model 


## The Meta Family of Models 

In this lesson, we will explore 2 models from the Meta family or "Llama Herd" - Llama 3.1 and Llama 3.2. The runnable code examples use Llama 3.3 and Llama 4, which are currently available alternatives in the Microsoft Foundry Models catalog.

These models come in different variants and are available in the [Microsoft Foundry Models catalog](https://ai.azure.com/catalog/models?WT.mc_id=academic-105485-koreyst).

> **Note:** GitHub Models is retiring at the end of July 2026. Here are more details on using [Microsoft Foundry Models](https://learn.microsoft.com/azure/ai-foundry/model-inference/overview?WT.mc_id=academic-105485-koreyst) to prototype with AI models.

---
> **Note:** The specific model versions this lesson was originally written against (Llama 3.1 70B/405B Instruct, Llama 3.2 11B/90B Vision Instruct) have since been retired from the Microsoft Foundry Models catalog. The code examples below use `Llama-3.3-70B-Instruct` and `Llama-4-Scout-17B-16E-Instruct` as currently available alternatives in the Microsoft Foundry Models catalog, so they still run today.

Model Variants (as originally covered in this lesson): 
- Llama 3.1 - 70B Instruct (retired) 
- Llama 3.1 - 405B Instruct (retired) 
- Llama 3.2 - 11B Vision Instruct (retired) 
- Llama 3.2 - 90B Vision Instruct (retired) 

---
Currently available alternatives used in the code examples: 
- Llama 3.3 - 70B Instruct (`Llama-3.3-70B-Instruct`) 
- Llama 4 Scout - 17B 16E Instruct (`Llama-4-Scout-17B-16E-Instruct`) 

*Note: The Llama 3 variants discussed above are retained for historical context and are no longer available in Microsoft Foundry Models.*

## Llama 3.1 

At 405 Billion Parameters, Llama 3.1 fits into the open source LLM category. 

The model is an upgrade to the earlier release Llama 3 by offering: 

- Larger context window - 128k tokens vs 8k tokens 
- Larger Max Output Tokens - 4096 vs 2048 
- Better Multilingual Support - due to increase in training tokens 

---
These enable Llama 3.1 to handle more complex use cases when building GenAI applications including: 
- Native Function Calling - the ability to call external tools and functions outside of the LLM workflow
- Better RAG Performance - due to the higher context window 
- Synthetic Data Generation - the ability to create effective data for tasks such as fine-tuning 

### Native Function Calling 

Llama 3.1 has been fine-tuned to be more effective at making function or tool calls. It also has two built-in tools that the model can identify as needing to be used based on the prompt from the user. These tools are: 

- **Brave Search** - Can be used to get up-to-date information like the weather by performing a web search 
- **Wolfram Alpha** - Can be used for more complex mathematical calculations so writing your own functions is not required. 

You can also create your own custom tools that the LLM can call. 

## Llama 3.2 

Despite being an LLM, one limitation of Llama 3.1 is its lack of multimodality. That is, the inability to use different types of input such as images as prompts and provide responses. This ability is one of the main features of Llama 3.2. These features also include: 

- Multimodality -  has the ability to evaluate both text and image prompts 
- Small to Medium size variations (11B and 90B) - this provides flexible deployment options, 
- Text-only variations (1B and 3B) - this allows the model to be deployed on edge / mobile devices and provides low latency 

The multimodal support represents a big step in the world of open source models.
