# Ansible Solution Template
[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://ms.portal.azure.com/#create/azure-oss.ansible)

This repository contains scripts to deploy [Ansible](https://www.ansible.com/) on Linux (Ubuntu 16.04 LTS) Virtual Machine on Azure, with Azure credential pre-configured.


## Customization
- Ansible Version  
  Fill in Ansible version(later than 2.5.0) to be installed, such as `2.7.4` or `latest`. Default is `latest`. You can get available release information from [here](https://github.com/ansible/ansible/releases).

- Azure Credential  
  Set Azure credentials from:
  - Not set.
  - Mannually setting service principal id and secret.
  - Enabling [Managed Service Identity](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview) on this VM. In this case, you will need to grant appriopriate role assignment to VM's system assigned identity, via az cli, portal or arm template, please refer to [this article](https://docs.microsoft.com/en-us/azure/role-based-access-control/role-assignments-portal) for more detail.




## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
