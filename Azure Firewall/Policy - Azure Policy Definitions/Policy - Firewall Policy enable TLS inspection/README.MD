## Azure firewall policy should enable TLS inspection within application rules

Enabling TLS inspection is recommended for all application rules to detect, alert, and mitigate malicious activity in HTTPS. To learn more about TLS inspection with Azure Firewall, visit https://aka.ms/fw-tlsinspect  

## Parameters  
Name:	Effect \
Type:	String \
Default Value:	Audit \
Allowed Values:	Audit; Deny; Disabled



More information : Azure [Built-in Policy](https://learn.microsoft.com/en-us/azure/governance/policy/samples/built-in-policies) to ensure [TLS inspection is enabled on Azure Firewall policy for Applicaton rules](https://ms.portal.azure.com/#view/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa58ac66d-92cb-409c-94b8-8e48d7a96596)  