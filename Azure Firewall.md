
FW should have a dedicated subnet so that it can have a VMSS in backend subscription

![enter image description here]([https://drive.google.com/file/d/1XP5wv82AAgC3CbH0cC1zA3sfsTApa7f7/view?usp=drive_link](https://drive.google.com/file/d/1XP5wv82AAgC3CbH0cC1zA3sfsTApa7f7/view))

**Creating AzureFirewallSubnet**

![Picture14](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/1c50051d-3cb3-4c02-998c-e8380da93e2f)

After creating a Subnet the error highlight gone and we can deploy FW

![Picture15](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/298a0a24-a3c8-493d-b0fb-ad47facfc49a)

Make note of private and public ip address of Firewall
Public ip address - 
Private ip address –
 
![Picture16](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/fac04c88-0fea-4385-bc01-56803b193e40)

![Picture17](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/48bb9abf-f4ed-469f-972c-b59b6743e7b2)

Create a route table and attached it to subnet of which needed to be protected

![Picture18](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/d4e3904f-598f-4177-8d4b-e5aca70565a5)

So we cannot associate route table to the AzureFirewallSubnet


![Picture19](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/b4644ad1-cc04-47aa-adc4-04c16ed05bc8)

Create route to Firewall private ip 
  
![Picture20](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/37e799c6-e658-4da0-9099-1b2575e10857)

Now go to Azure firewall policy and configure Application rules and network rules and dnat 
Application rule to allow http and https 
Network rule to allow DNS (53) or you can also point to custom dns server
DNAT rules for RDP rule (Point the destination translation type to VM private ip)

![Picture21](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/89235780-14d0-47eb-8dac-64c61ff2cc77)

![Picture22](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/09af7dfd-b99b-450c-8db4-6f17741b7a96)
 
Lets test the computer behind the firewall with RDP     
 
<img width="463" alt="Picture23" src="https://github.com/Shroov3/Journey-of-Azure/assets/113405359/c31430cf-6800-4d82-8e34-e714501535f7">

**END!**
