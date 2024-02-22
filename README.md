# Microsoft Azure OpenAI

I have created a new GitHub repository named 'Microsoft Azure OpenAI' to show Azure policies for OpenAI. The repository is set up to store Azure Policy definitions and related resources for governing OpenAI services on the Azure platform. Feel free to contribute or collaborate on defining and enforcing policies that align with OpenAI's security and compliance requirements.

<h2>Microsoft Article for Open AI</h2>

[Monitoring Azure OpenAI (microsoft.com)](https://techcommunity.microsoft.com/t5/fasttrack-for-azure/azure-openai-insights-monitoring-ai-with-confidence/ba-p/4026850)

[Security Best Practices for GenAI Applications (OpenAI) in Azure](https://techcommunity.microsoft.com/t5/azure-architecture-blog/security-best-practices-for-genai-applications-openai-in-azure/ba-p/4027885)

# Azure Policies

Here are some policies to enforce for Open AI Security and Compliance:
  
-[Deploy Diagnostic Settings for Azure OpenAI to Log Analytics workspace (Custom Built)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/diagnosticsettings.json)

-Permit only approved OpenAI models (Custom/Community)

-Audit OpenAI instances with content filtering enabled (Custom/Community)

-Audit OpenAI instances public access enabled (Custom/Community)

-Container :Azure Container Instance container group should deploy into a virtual network (Builtin or Custom)

-Network Security Group: Create NSG and Attach to Existing Subnet (Custom Built)

-Network Security Group:Flow logs should be configured for every network security group (Builtin or Custom)

-Load Bal: Deploy Diagnostic Settings for Load Balancer to Log Analytics workspace (Builin or Custom)

-Public IP: Enable logging by category group for Public IP addresses (microsoft.network/publicipaddresses) to Log Analytics (Builtin or Custom)
