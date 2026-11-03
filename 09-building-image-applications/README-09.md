---
marp: true
---
<!-- headingDivider: 3 -->
<!-- paginate: true -->


# Building Image Generation Applications

## Introduction

Image generation lets you turn a natural-language prompt into a picture. In this lesson we work with the **`gpt-image`** family of models from OpenAI - the current generation of image models available on **[Microsoft Foundry](https://ai.azure.com?WT.mc_id=academic-105485-koreyst)** and the OpenAI platform. These models replace the older DALL·E models (DALL·E 2/3 are legacy).

Throughout the lesson we use a fictitious startup, **Edu4All**, that builds learning tools. The team wants to generate illustrations for assignments and study materials.

## Learning goals

By the end of this lesson you'll be able to:

- Explain what image generation is and where it's useful.
- Understand the `gpt-image` model family and how it differs from the legacy DALL·E models.
- Build an image generation app in Python (and TypeScript / .NET).
- Edit images and apply safety guardrails with metaprompts.

## What is image generation?

Image generation models create images from a text prompt. Modern models such as `gpt-image` are built on transformer + diffusion techniques: the model learns the relationship between text and images during training, then, given a prompt, iteratively "denoises" random noise into an image that matches the description.

---
Two well-known families of image models are:

- **`gpt-image` (OpenAI)** - the current generation, used in this lesson. It supports text-to-image generation and image editing (inpainting with a mask).
- **Midjourney** - a popular third-party model with its own service and Discord-based workflow.

> Older OpenAI image models - **DALL·E 2** and **DALL·E 3** - are legacy. DALL·E 3 is no longer available for new deployments, and features like `create_variation` only existed in DALL·E 2. Use the `gpt-image` models for new applications.

### Which `gpt-image` model should I use?

On Microsoft Foundry the following are **Generally Available**:

| Model | Notes |
| --- | --- |
| **`gpt-image-2`** | The latest and most capable image model - recommended default. |
| `gpt-image-1.5` | Generally available; strong quality at lower cost. |
| `gpt-image-1-mini` | Generally available; fastest / lowest cost. |
| `gpt-image-1` | Preview only. |

---
Always check the current [Foundry image models list](https://learn.microsoft.com/azure/ai-foundry/openai/concepts/models?WT.mc_id=academic-105485-koreyst) for availability and regions.

> **Important:** `gpt-image` models return the generated image as **base64** (`b64_json`), not as a URL. Your code decodes the base64 string to bytes and saves it - there's no image URL to download.
