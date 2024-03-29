# Policy - Public IP addresses should have resource logs enabled for Azure DDoS Protection Standard


Enable resource logs for public IP addressess in diagnostic settings to stream to a Log Analytics workspace. Get detailed visibility into attack traffic and actions taken to mitigate DDoS attacks via notifications, reports and flow logs.


## Parameters
Name:	Effect  \
Type:	String  \
Default Value:	AuditIfNotExists  \
Allowed Values:	AuditIfNotExists; DeployIfNotExists; Disabled  \  

Name:	Diagnostic setting name  \
Type:	String  \  

Name:	Log Analytics workspace  \
Type:	String  \  

Name:	Enable Logs  \
Type:	String  \
Default Value:  True  \
Allowed Values:	True; False  \  

Name:	Enable Metrics  \
Type:	String  \
Default Value:	False  \
Allowed Values:	True; False  \  

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit <https://cla.opensource.microsoft.com>.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

