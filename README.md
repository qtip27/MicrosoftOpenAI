# Microsoft Azure OpenAI

I have created a new GitHub repository named 'Microsoft Azure OpenAI' to show Azure policies for OpenAI. The repository is set up to store Azure Policy definitions and related resources for governing OpenAI services on the Azure platform. Feel free to contribute or collaborate on defining and enforcing policies that align with OpenAI's security and compliance requirements.

<h2>Microsoft Article for Open AI</h2>

[Monitoring Azure OpenAI (microsoft.com)](https://techcommunity.microsoft.com/t5/fasttrack-for-azure/azure-openai-insights-monitoring-ai-with-confidence/ba-p/4026850)

[Security Best Practices for GenAI Applications (OpenAI) in Azure](https://techcommunity.microsoft.com/t5/azure-architecture-blog/security-best-practices-for-genai-applications-openai-in-azure/ba-p/4027885)

# Azure Policies

📄 Here are some policies to enforce for Open AI Security and Compliance:
  
[Deploy Diagnostic Settings for Azure OpenAI to Log Analytics workspace (Custom Built)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/diagnosticsettings.json)

Description: Deploys the diagnostic settings for Azure OpenAI to stream to a Log Analytics workspace when any Azure OpenAI which is missing this diagnostic settings is created or updated. The Policy will set the diagnostic with all metrics and category enabled



[Permit only approved OpenAI models (Custom/Community)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/OpenAI_models.json)

Description: This policy permits only certain types of OpenAI models to be deployed


[Audit OpenAI instances with content filtering enabled (Custom/Community)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/OpenAI_instances.json)

Description: Azure OpenAI Service includes a content management system that filters content. If you are working with sensitive data, content filtering should be disabled so that Microsoft is not processing your data.


[Audit OpenAI instances public access enabled (Custom/Community)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/public_access.json)

Description: Azure OpenAI instances should not have public access enabled. Open AI instances should only be accessible via select networks or a private endpoint.



-Container :Azure Container Instance container group should deploy into a virtual network (Builtin or Custom)

-Network Security Group: Create NSG and Attach to Existing Subnet (Custom Built)

-Network Security Group:Flow logs should be configured for every network security group (Builtin or Custom)

-Load Bal: Deploy Diagnostic Settings for Load Balancer to Log Analytics workspace (Builin or Custom)

-Public IP: Enable logging by category group for Public IP addresses (microsoft.network/publicipaddresses) to Log Analytics (Builtin or Custom)
