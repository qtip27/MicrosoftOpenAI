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


[Container Instances: Azure Container Instance container group should deploy into a virtual network (Builtin or Custom)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/Container_Instance.json)

Description: Secure communication between your containers with Azure Virtual Networks. When you specify a virtual network, resources within the virtual network can securely and privately communicate with each other.


[Network Security Group: Create NSG and Attach to Existing Subnet (Custom Built)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/Network_Security.json)

Description: "lThis policy checks for an existing Virtual Network and Subnet, creates a Network Security Group if it doesn't exist, and attaches it to the existing Subnet.


[Network Security Group:Flow logs should be configured for every network security group (Builtin or Custom)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/Flow_Logs.json)

Description: Audit for network security groups to verify if flow logs are configured. Enabling flow logs allows to log information about IP traffic flowing through network security group. It can be used for optimizing network flows, monitoring throughput, verifying compliance, detecting intrusions and more.


[Load Bal: Deploy Diagnostic Settings for Load Balancer to Log Analytics workspace (Builin or Custom)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/LB_Diagnostic.json)

Description: Deploys the diagnostic settings for Load Balancer to stream to a Log Analytics workspace when any Load Balancer which is missing this diagnostic settings is created or updated. The Policy will set the diagnostic with all metrics and category enabled.


[Public IP: Enable logging by category group for Public IP addresses (microsoft.network/publicipaddresses) to Log Analytics (Builtin or Custom)](https://github.com/qtip27/MicrosoftOpenAI/blob/main/IP_Analtics.json)

Description: Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for Public IP addresses (microsoft.network/publicipaddresses).

# Non-Compliant Policies

If your looking for a way to get notified of your polcies not being compliance, you can use this article below to setup the alerts for this:

[Azure Monitoring alerting rule to notify on non-compliant resources](https://msandbu.org/azure-monitoring-alerting-rule-to-notify-on-non-compliant-resources/)
