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
  
<img src="https://user-images.githubusercontent.com/104326475/175784293-aeed1bdb-c90e-4c8d-b0d7-6a2ce53859b9.png" height="185%" width="185%" alt="Azure Policies"/>

<p/>


# Admins will be able to see in the overview section which policies were triggers
- Here we can see that the VMs that we created are non-compliant under IaaSmAntimalware extension
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175785259-16099dc0-e3b2-4191-80bd-dfb28f0beaef.png" height="185%" width="185%" alt="Azure Policies"/>

<p/>


