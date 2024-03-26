# A Step-by-Step Guide to Setup Honeypot Using Azure Sentinel

## Basic Overview:

A Step-by-Step guide to deploy a windows based honeypot server on microsoft azure cloud. Open all the firewalls and log all the failed login attempts using a custom powershell script. Use Azure Sential to create a map of all the failed login attempts.


## Step 1: Create a Azure account

Create a Azure account by visiting this [Azure Link](https://azure.microsoft.com/en-ca/free/search/?ef_id=_k_CjwKCAjw5ImwBhBtEiwAFHDZx5oI3jzvCW0aB-60E-an_0h9v9VlFNKXgP2E2CuI_1HxantKOOxLvhoCqWsQAvD_BwE_k_&OCID=AIDcmmqz3gd78m_SEM__k_CjwKCAjw5ImwBhBtEiwAFHDZx5oI3jzvCW0aB-60E-an_0h9v9VlFNKXgP2E2CuI_1HxantKOOxLvhoCqWsQAvD_BwE_k_&gad_source=1&gclid=CjwKCAjw5ImwBhBtEiwAFHDZx5oI3jzvCW0aB-60E-an_0h9v9VlFNKXgP2E2CuI_1HxantKOOxLvhoCqWsQAvD_BwE).

DO NOTE: You need a valid credit card to setup the account and get the $200 free credit. The credits are only valid for 30 days.

![1711475194853](image/guide/1711475194853.png)

## Step 2: Creating a Virtual Machine

Once the azure account is up and running, next step is to deploy a virtual machine.

* Go to `https://portal.azure.com/#home`
* Login into your Azure account and search for "Virtual machine" in the search
* Select `Azure virtual machine`
