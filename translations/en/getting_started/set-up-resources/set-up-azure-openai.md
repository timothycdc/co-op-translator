<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "10d8cb07ad0d2ee6705439d4e382ecc9",
  "translation_date": "2025-05-06T18:14:35+00:00",
  "source_file": "getting_started/set-up-resources/set-up-azure-openai.md",
  "language_code": "en"
}
-->
# Set up Azure OpenAI for language translation

## Create an Azure OpenAI resource in Azure AI Foundry

To set up Azure OpenAI in Azure AI Foundry, follow these steps:

### Creating a Hub

1. Sign in to the [Azure AI Foundry portal](https://ai.azure.com): Make sure you're signed in with your Azure account.

2. Navigate to the Management Center: From the home page, select "Management Center" from the left menu.

3. Create a New Hub: Click on "+ New hub" and enter the necessary details such as Subscription, Resource Group, and Hub Name. We recommend deploying the hub to East US as this region supports Cognitive Vision and GPT models.

4. Review and Create: Review the details and click "Create" to set up your hub.

### Creating a Project

1. Go to the Home Page: If you're not already there, select "Azure AI Foundry" at the top left of the page to go to the home page.

2. Create a Project: Click on "+ Create project" and enter a name for your project.

3. Select a Hub: If you have multiple hubs, select the one you want to use. If you want to create a new hub, you can do so during this step.

4. Configure the Project: Follow the prompts to configure your project according to your needs.

5. Create the Project: Click "Create" to finalize the setup.

### Deploying a Model and Endpoint for OpenAI model

1. Sign in to the [Azure AI Foundry portal](https://ai.azure.com): Make sure you're signed in with the Azure subscription that has your Azure OpenAI Service resource.

2. Navigate to Models and Endpoint: From the Azure AI Foundry home page, find the tile that says " and select "Let's go." or Model and Endpoints in the left-hand menu.

3. If you don’t already have a GPT Model deployed, select deploy model: choose a GPT model. We recommend GPT-4o, GPT-4o-mini, or o3-mini.

4. Access your resources: You should see your existing Azure OpenAI Service resources. If you have multiple resources, use the selector to choose the one you want to work with.

For more detailed instructions, you can refer to the official Azure AI Foundry documentation.

[How to Create a project](https://learn.microsoft.com/azure/ai-studio/how-to/create-project)

[How to Create resources](https://learn.microsoft.com/azure/ai-studio/how-to/create-azure-ai-resource)

[How to use OpenAI Model in AI Foundry](https://learn.microsoft.com/azure/ai-studio/ai-services/how-to/connect-azure-openai)

[OpenAI Services in Azure AI Foundry](https://learn.microsoft.com/azure/ai-studio/azure-openai-in-ai-studio)

**Disclaimer**:  
This document has been translated using the AI translation service [Co-op Translator](https://github.com/Azure/co-op-translator). While we strive for accuracy, please be aware that automated translations may contain errors or inaccuracies. The original document in its native language should be considered the authoritative source. For critical information, professional human translation is recommended. We are not liable for any misunderstandings or misinterpretations arising from the use of this translation.