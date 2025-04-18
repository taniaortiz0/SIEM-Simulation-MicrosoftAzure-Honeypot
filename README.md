# SIEM-Simulation-with-Microsoft-Azure

![List of Resource Groups](https://github.com/user-attachments/assets/9e3704d4-e7c8-43ca-9538-410b3ba76ed3)

Created a list of Resources for the SOC Lab involving a Resource group to store Azure services such as Windows 10 VM, Virtual network, Log Analytics workspace, and Microsoft Sentinel. 

![Allowing any ports access](https://github.com/user-attachments/assets/74e0e276-9066-4360-8de0-f0163d769c5b) 

After creating the list of resources, I then configured the Network security group to allow any ports in to see the amass of incoming traffic.


![Windows Firewall Set OFF](https://github.com/user-attachments/assets/7704e0c5-1678-404b-bd15-348b0f0b1bc7)

In the Windows 10 VM I created, (connection via RDP) I have configured the firewall settings to be set OFF. 

![AMA setup](https://github.com/user-attachments/assets/e9c2e3cd-3f69-4593-8ad5-1e38979b43d9)

I went to the Microsoft Sentinel services page, created a workspace, installed two Data connectors (Security Events via Legacy Agent and Windows Security Events via AMA), and created a data collection rule for my virtual machine to forward logs to the Log Analytics workspace.

![Using KQL to see events](https://github.com/user-attachments/assets/b7b10b9f-f480-49fd-b31f-6073db38e307)

Querying the Log Analytics workspace using KQL to view Security Events with certain filters to view logs in real-time. 
