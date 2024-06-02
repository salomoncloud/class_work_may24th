this is the homework assignment for the 31st of May. This file has been created and committed locally as asked. 

Here is a list of Azure commands that will come in handy;

Basic Commands:

Login to Azure
az login

Set the subscription you want to use
az account set --subscription "Your-Subscription-Name"
List all available subscriptions
az account list --output table

Resource Group Commands:
Create a resource group
az group create --name MyResourceGroup --location eastus

List resource groups
az group list --output table

Delete a resource group
az group delete --name MyResourceGroup --yes --no-wait

Virtual Machine (VM) Commands:

Create a virtual machine
az vm create --resource-group MyResourceGroup --name MyVM --image UbuntuLTS --admin-username azureuser --generate-ssh-keys

List all virtual machines
az vm list --output table

Start a virtual machine
az vm start --resource-group MyResourceGroup --name MyVM

Stop a virtual machine
az vm stop --resource-group MyResourceGroup --name MyVM

Delete a virtual machine
az vm delete --resource-group MyResourceGroup --name MyVM --yes

Storage Account Commands:

Create a storage account
az storage account create --name mystorageaccount --resource-group MyResourceGroup --location eastus --sku Standard_LRS

List storage accounts
az storage account list --output table

Delete a storage account
az storage account delete --name mystorageaccount --resource-group MyResourceGroup --yes

Networking Commands:

Create a virtual network (VNet)
az network vnet create --resource-group MyResourceGroup --name MyVNet --address-prefix 10.0.0.0/16

Create a subnet
az network vnet subnet create --resource-group MyResourceGroup --vnet-name MyVNet --name MySubnet --address-prefix 10.0.0.0/24

Create a network security group (NSG)
az network nsg create --resource-group MyResourceGroup --name MyNSG

Create a network interface (NIC)
az network nic create --resource-group MyResourceGroup --vnet-name MyVNet --subnet MySubnet --name MyNic

SQL Database Commands:

Create a SQL server
az sql server create --name mydemoserver --resource-group MyResourceGroup --location eastus --admin-user myadmin --admin-password mypassword

Create a SQL database
az sql db create --resource-group MyResourceGroup --server mydemoserver --name mydatabase --service-objective S0

List SQL databases
az sql db list --resource-group MyResourceGroup --server mydemoserver --output table

Delete a SQL database
az sql db delete --resource-group MyResourceGroup --server mydemoserver --name mydatabase --yes

Azure Kubernetes Service (AKS) Commands:

Create an AKS cluster
az aks create --resource-group MyResourceGroup --name MyAKSCluster --node-count 1 --enable-addons monitoring --generate-ssh-keys

Get credentials for the AKS cluster
az aks get-credentials --resource-group MyResourceGroup --name MyAKSCluster

List AKS clusters
az aks list --output table

Delete an AKS cluster
az aks delete --resource-group MyResourceGroup --name MyAKSCluster --yes --no-wait