# Policy-Service

# What is the Azure Policy Service?
- Policy service is another security feature that allows admins to impose restrictions on Azure resources
- There are a ton of built-in policies and they are used from a governance perspective
- Admins can also create custom policies
- Examples: Ensuring all VMs have Antimalware extension installed or ensuring all resource groups have tags in place.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175575028-8e26cacd-74f1-478b-b91c-450aadd351a5.png" height="55%" width="55%" alt="Azure Policies"/>

<p/>

# Create two virtual machines and apply an azure policy that ensures antimalware extension is installed on the VMs 


# Navigate to Azure Policies and apply Antimalware policies
- Admins can apply policies at the suscription or resource group level and exclude a specific resource group

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175784170-70184d0c-a728-4543-9b15-11b78f5b32f1.png" height="185%" width="185%" alt="Azure Policies"/>

<p/>

# Assign the IaaSAntimalware Extension policy to your subscription
- This policy checks that VMs in the subscription have the extension installed.
- Reminder - we assigned this policy at the subscription level. 
- We could exclude particular resource groups if we wanted to.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175784224-9a282209-6157-467f-9b7c-041653473216.png" height="185%" width="185%" alt="Azure Policies"/>

<p/>
