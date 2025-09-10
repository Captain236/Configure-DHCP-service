# Configure-DHCP-service

**Dynamic Host Configuration Protocol (DHCP) – Automated IP Address Management DHCP (Dynamic Host Configuration Protocol) is a network management protocol that automatically assigns IP addresses, subnet masks, default gateways, and DNS settings to devices on a network. This eliminates the need for manual IP configuration, ensuring efficient and conflict-free network management.**

Key Benefits:

**✅ Automated IP Assignment – Reduces manual configuration and errors.**

**✅ Efficient IP Management – Dynamically allocates and reclaims unused IP addresses.**

**✅ Scalability – Ideal for networks with a large number of devices.**

**✅ Centralized Control – Simplifies administration with a dedicated DHCP server.**

## Summary
**In this project, I installed and configured the DHCP protocol on Windows Server. I created an IP address pool, allowing the DHCP server to automatically assign IP addresses to client machines, ensuring efficient and dynamic network management.**

## Step - 1
<img width="1485" height="882" alt="1 (2)" src="https://github.com/user-attachments/assets/193f1e8e-60d9-4f63-9a10-fc4d6019d951" />

**ii. In "Server Roles," select and add the DHCP Server role.**
<img width="1453" height="636" alt="2 (2)" src="https://github.com/user-attachments/assets/cf552800-3aab-49d6-ae8d-fddff5cd1da4" />

**iii. In the "Confirmation" section, click "Install" to set up the DHCP Server.**
<img width="1455" height="643" alt="3 (2)" src="https://github.com/user-attachments/assets/d0df0149-d956-4b4e-b16e-785a64cb72e0" />

**iv. Once the installation is complete, click on "Complete DHCP Configuration" and follow the steps as shown in the screenshots.**
<img width="1471" height="641" alt="4 (2)" src="https://github.com/user-attachments/assets/fb0a8b09-9fba-4174-a451-f0a6e580fd7f" />
<img width="1311" height="638" alt="5 (2)" src="https://github.com/user-attachments/assets/630a7a3c-f04e-4130-abbb-affea707b64a" />
<img width="1422" height="645" alt="6 (2)" src="https://github.com/user-attachments/assets/47138ca4-5327-4001-86ed-19fb5bcdc090" />
<img width="1201" height="641" alt="7 (2)" src="https://github.com/user-attachments/assets/531adc31-3a52-4553-ac39-9e8b1078e573" />

## Step - 2

**i. Go to "Tools" in Server Manager and select "DHCP."**
<img width="884" height="708" alt="8 (2)" src="https://github.com/user-attachments/assets/fa8c4228-c286-4d85-9ac7-d49082d4b997" />

**ii. To add an IPv4 scope, right-click on "IPv4" and select "New Scope."**
<img width="722" height="746" alt="9 (2)" src="https://github.com/user-attachments/assets/7627e1a2-aef6-4eaf-88d0-49dc351407b2" />

**iii. Enter a name of your choice for the scope and click "Next."**
<img width="980" height="499" alt="10 (2)" src="https://github.com/user-attachments/assets/d44bdf5d-1c5c-4870-931c-2f51a7256505" />

**iv. Specify the Start and End IP range for the scope and click "Next."**
<img width="1075" height="497" alt="11 (2)" src="https://github.com/user-attachments/assets/28290ead-2a9b-4cf3-a226-9330e35842a8" />

**v. In "Add Exclusion and Delay," skip assigning any excluded IPs and proceed by clicking "Next."**

WHat is Add Exclusion and Delay in DHCP??

Exclusion: Reserves specific IPs so the DHCP server doesn’t assign them, ensuring static IPs for critical devices.

Delay: Adds a response delay in multi-DHCP setups, allowing the preferred server to assign IPs first.
<img width="967" height="485" alt="12 (1)" src="https://github.com/user-attachments/assets/12a9dd49-11f1-4967-8d8b-90f67b78345a" />

**vi. What is Lease Duration?**

Lease Duration defines how long a device can use an assigned IP address before it must renew the lease. Shorter durations suit dynamic networks (e.g., Wi-Fi hotspots), while longer durations are ideal for stable environments (e.g., offices).
<img width="971" height="487" alt="13 (2)" src="https://github.com/user-attachments/assets/f918774f-1021-4578-86ee-9a5d917c4f6a" />

**vii. Enter the Default Gateway IP address and click "Next."**
<img width="969" height="492" alt="14 (2)" src="https://github.com/user-attachments/assets/faeb4d5f-3bce-48e8-ad1f-2e315859be1b" />

**viii. Click "Next" through the remaining steps until you reach "Finish."**
<img width="962" height="489" alt="15 (2)" src="https://github.com/user-attachments/assets/179ce39f-ca9a-47e9-be2c-92ca312c874a" />

## Step - 3

**i. Now lets assign the DHCP IP address to our machine , for this type this command**
<img width="448" height="250" alt="16 (1)" src="https://github.com/user-attachments/assets/74a0e9b8-7856-47b9-8263-f3af9a61d26b" />

**ii. Go to "Network Properties," select your network adapter, then click on "Internet Protocol Version 4 (TCP/IPv4)."**
<img width="966" height="674" alt="17" src="https://github.com/user-attachments/assets/640f502e-5fd6-41a0-ad43-2188effc4572" />

**iii. Select "Obtain an IP address automatically" and "Obtain DNS server address automatically," then click "OK."**
<img width="966" height="674" alt="17" src="https://github.com/user-attachments/assets/d7307aac-59f5-4d76-9877-ce7810bd146c" />

**After this, check the network status—you will see that the IP address has been dynamically assigned by the DHCP server.**
















