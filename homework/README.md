**Data Source: azurerm_resource_group**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/resource_group

Description: Use this data source to access information about an existing Resource Group.

To create a resource group on Azure:
![image](https://github.com/salomoncloud/class_work_may24th/assets/158000174/418985b2-2ccb-4d84-8722-146868ea8c9c)


Make sure you enter name & location


**Data Source: azurerm_subnet**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/subnet

Description: Use this data source to access information about an existing Subnet within a Virtual Network.

To create a new subnet on Azure:
![image](https://github.com/salomoncloud/class_work_may24th/assets/158000174/958b1a7b-3a0b-4877-ab5c-372aa9990e37)


**resource "azurerm_public_ip"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/public_ip

Description: Manages a Public IP Address.

To create a public IP address on Azure:
![image](https://github.com/salomoncloud/class_work_may24th/assets/158000174/73d9c627-3a95-44bf-b552-04edc2890db4)


Make sure to complete all fields with a red *

**resource "azurerm_lb"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb

Description: Manages a Load Balancer Resource.

To create a load balancer on Azure:
![image](https://github.com/salomoncloud/class_work_may24th/assets/158000174/f77016d4-9c51-447a-99ed-dc6ce3c0f117)


Make sure you enter:
- resource group name
- name
- location
- SKU (Standard/Gateway/Basic)
- Type (Public/Internal)
- Tier (Regional/Global)


**resource "azurerm_lb_backend_address_pool"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_backend_address_pool_address

Description: Manages a Backend Address within a Backend Address Pool.


**resource "azurerm_lb_nat_rule"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_nat_rule.html

Description: Manages a Load Balancer NAT Rule.


**resource "azurerm_lb_probe"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/2.99.0/docs/resources/lb_probe

Description: Manages a LoadBalancer Probe Resource.


**resource "azurerm_lb_rule"**

Link: https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_rule.html

Description: Manages a Load Balancer Rule.
