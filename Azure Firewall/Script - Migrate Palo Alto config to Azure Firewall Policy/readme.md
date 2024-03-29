# Import Palo Alto Panorama policy into Azure Firewall Policy

This script will export Palo Alto firewall ruleset to be used in creating an Azure Firewall policy.  
You can find more information about the process in this [blogpost](https://github.com/erjosito) created by a community member

The script will generate an ARM template that contains either a full Azure Policy with a Rule Collection Group containing the translated rules, or just the Rule Collection Group that you can deploy to an existing policy. To generate the policy, you just specify JSON as the output format, optionally the flag --pretty to make it more human readable, and write to a file:

    python3 ./pa2azfw.py --log-level 4 --output json --use-ip-groups --pretty >pa-policy.json

When deploying the generated output json file content into Azure, the Address Groups will be transformed into Azure IP Groups. 
The policies will be transformed into Azure Firewall network rules that leverage the previously created address groups. The services and service groups will be expanded into the corresponding protocol and port fields for each rule, since there is not an equivalent concept in Azure.  

## Contributing
This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.ls

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
