<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.12.26 |
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | >= 2.54.0 |

## Providers

No providers.

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_data_connector_confluence_audit"></a> [data\_connector\_confluence\_audit](#module\_data\_connector\_confluence\_audit) | ../sentinel-data-connector-arm-generic | n/a |

## Resources

No resources.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_access_token"></a> [access\_token](#input\_access\_token) | Confluence access\_token for audit stream | `string` | n/a | yes |
| <a name="input_arm_template"></a> [arm\_template](#input\_arm\_template) | The ARM template URL to download the template from. | `string` | `"https://raw.githubusercontent.com/Azure/Azure-Sentinel/9218a8839d6b8b2d95ee426b97a7f1fd6744ae45/DataConnectors/AtlassianConfluenceAudit/azuredeploy_Connector_ConfluenceAuditAPI_AzureFunction.json"` | no |
| <a name="input_homesite_name"></a> [homesite\_name](#input\_homesite\_name) | https://HOMESITENAME.atlassian.net | `string` | n/a | yes |
| <a name="input_name"></a> [name](#input\_name) | The name which should be used for this Confluence Audit Data Connector. | `string` | n/a | yes |
| <a name="input_resource_group_name"></a> [resource\_group\_name](#input\_resource\_group\_name) | The name of the Resource Group where the Resource Group Template Deployment should exist. | `string` | n/a | yes |
| <a name="input_username"></a> [username](#input\_username) | Confluence username for audit stream | `string` | n/a | yes |
| <a name="input_workspace_id"></a> [workspace\_id](#input\_workspace\_id) | The ID of the Log Analytics Workspace that this Confluence Audit Data Connector resides in. | `string` | n/a | yes |
| <a name="input_workspace_key"></a> [workspace\_key](#input\_workspace\_key) | The key of the Log Analytics Workspace that this Confluence Audit Data Connector resides in. | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id"></a> [id](#output\_id) | The ID of the Resource Group Template Deployment. |
| <a name="output_output_content"></a> [output\_content](#output\_output\_content) | The JSON Content of the Outputs of the ARM Template Deployment. |
<!-- END_TF_DOCS -->
