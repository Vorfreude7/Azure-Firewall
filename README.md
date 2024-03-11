# Azure-Firewall

## Tasks
#Task 1: Use a template to deploy the lab environment.

#Task 2: Deploy an Azure firewall.

#Task 3: Create a default route.

#Task 4: Configure an application rule.

#Task 5: Configure a network rule.

#Task 6: Configure DNS servers.

#Task 7: Test the firewall.

### Skills Learned
- Enhanced knowledge of network and application firewall rules.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
-Microsoft Azure

-Azure Firewall

## Steps
#Task 1: Use a template to deploy the lab environment.

I used the template provided to deploy a lab environment on Azure. This is done by deploying a custom template, and loading the json file provided
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/bb9b644a-dbde-4bf1-952c-b01c40328b58)


#Task 2: Deploy an Azure firewall.

I deployed an Azure Firewall.
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/ee2a6841-eb67-4762-acd1-6f6577252a9b)

#Task 3: Create a default route.

I configured a default route for the Workload-SN subnet. This route will configure outbound traffic through the firewall.
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/56ef3af5-903c-49e0-a115-5e77649166f5)

#Task 4: Configure an application rule.

Below is the Application rule that I configured. This rule allows 10.0.2.0/24 subnet to reach www.bing.com on port 80 and 443.
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/d73f6883-19c3-4dff-8b3b-5049384317b5)


#Task 5: Configure a network rule.
The network rule that I configured below, allows 10.0.2.0/24 subnet to reach the DNS Servers that is 209.244.0.3 and 209.244.0.4 on port 53.
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/b65cf17b-fca2-4d66-8cd9-09ce1cc9eb60)


#Task 6: Configure DNS servers.

I configured primary and Secondary DNS Servers for the Virtual machine Srv-Work
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/42267faf-24a0-4024-b07e-c9166da6be12)


#Task 7: Test the firewall.
I was able to access www.bing.com, because of the application rule configured earlier that allows that traffic
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/7710c878-effd-47e7-bd2e-2b9e118a571d)

Traffic to microsoft.com is however being blocked because there is no rule configured to allow that traffic.
![image](https://github.com/Vorfreude7/Azure-Firewall/assets/128520269/9837ad73-8bed-45f1-a7bd-889c04a0727b)





