## Enable Rate Limit rule to protect against DDoS attacks on Azure Front Door WAF

The Azure Web Application Firewall (WAF) rate limit rule for Azure Front Door controls the number of requests allowed from a particular client IP address to the application during a rate limit duration.  

## Parameters
Name:	Effect \
Type:	String \
Default Value:	Audit \
Allowed Values:	Audit; Deny; Disabled  


More information : Azure [Built-in Policy](https://learn.microsoft.com/en-us/azure/governance/policy/samples/built-in-policies) to enable [Rate limit rules for WAF on Azure Front Door](https://ms.portal.azure.com/#view/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe52e8487-4a97-48ac-b3e6-1c3cef45d298)  