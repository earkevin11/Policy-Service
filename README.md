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
  
<img src="https://user-images.githubusercontent.com/104326475/175785326-868ff501-9d7c-417f-9cf5-3c975e8e4e9f.png" height="195%" width="185%" alt="Azure Policies"/>

<p/>


# Azure Policy Remediation
- Admins can now remediate these policies by deploying another policy that will deploy the antimalware extension
- In the policy definition, it will execute if the extension does not exist on Windows Server 2019


<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175785387-2bccbd96-6ccd-4cf6-ac7b-c66cf13fe0de.png" height="75%" width="75%" alt="Azure Policies"/>

<p/>


# Deploy the IaaSAntimalware extension for Windows Server
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175785437-2004e2f5-a917-4270-ad0c-b10981b73859.png" height="75%" width="75%" alt="Azure Policies"/>

<p/>



# For existing resources like the VMs we created that are non compliant, a remediation task is needed
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/175785602-bfa7838a-5d95-4562-a8c3-3b482c6d577b.png" height="75%" width="75%" alt="Azure Policies"/>

<p/>





