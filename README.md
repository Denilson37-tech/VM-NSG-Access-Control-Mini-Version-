Securing an Azure Virtual Machine with Network Security Groups

Project Story

I had a virtual machine running in Azure. Without security controls in place, it was exposed to the internet and could be targeted by unauthorized users.

In real cloud environments, misconfigured network access is a common source of compromise. My goal in this project was to secure that VM by restricting inbound network access with a Network Security Group.

NSGs act as a firewall for Azure resources and let me control traffic in and out of a VM at the network layer.

What I Built

I created an NSG and applied it to the VM so that only trusted traffic is allowed. I reviewed the default rules, added specific security rules, and tested that traffic was blocked or allowed as intended.

Step 1: Create or Identify the VM

I used the Azure portal to create a virtual machine or select an existing one.

Screenshot 1 shows the VM overview page and proves the VM is running in Azure

Step 2: Apply a Network Security Group

I created a Network Security Group and attached it to the VM’s network interface or subnet.

I reviewed the default NSG rules to understand the initial exposure
I added custom rules to restrict access

Example custom rules I created

Allow RDP (3389) only from my trusted IP address so only I can manage the VM
Allow HTTP (80) for test purposes from trusted sources
All other inbound traffic blocked by default

Screenshot 2 shows the NSG rules applied to the VM

Step 3: Test Access

I validated that the rules worked

Accessing the VM from my trusted IP with RDP worked
Accessing from another IP was blocked

Screenshot 3 shows the test results with allowed and blocked traffic

Why This Matters

Network Security Groups are fundamental to protecting workloads in Azure. They control traffic to and from resources

Any open or poorly restricted port increases risk
Restricting access reduces the attack surface
Testing traffic proves the controls are effective

This is how teams secure VMs in real environments

Outcome

Restricting network access to trusted sources reduces the risk of unauthorized login attempts and internet exposure

This project shows practical Azure network security skills and demonstrates that I understand how to protect cloud resources
