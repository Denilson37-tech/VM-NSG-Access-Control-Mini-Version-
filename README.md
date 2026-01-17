Securing an Azure Virtual Machine with Network Security Groups (NSG)

This project started with a simple problem.
A virtual machine in Azure was running, but the network was wide open. Anyone could attempt to connect. This is how real cloud breaches begin.

As a junior Azure security engineer, my responsibility is not to build complex systems. My responsibility is to reduce obvious risk.

So I focused on one thing.
Control who can talk to the VM and who cannot.

I used a Network Security Group to define inbound and outbound rules. Only required traffic was allowed. Everything else was denied by default.

This mirrors real-world environments where misconfigured NSGs expose workloads to the internet.

What I Did in This Project

I created a virtual machine in Azure
I attached a Network Security Group (NSG) to the VM
I reviewed the default rules to understand existing exposure
I created custom inbound rules to restrict access
I validated that only permitted traffic could reach the VM

What I Did in This Project

I created a virtual machine in Azure
I attached a Network Security Group (NSG) to the VM
I reviewed the default rules to understand existing exposure
I created custom inbound rules to restrict access
I validated that only permitted traffic could reach the VM
I documented the project and included screenshots

Explain each rule

Allowed RDP (3389) only from my IP to prevent unauthorized login

Allowed HTTP (80) only for testing purposes

Blocked all other inbound traffic by default

Validation / Testing

Attempted RDP from allowed IP → connected successfully

Attempted RDP from a different IP → connection blocked

This proves the rules work as intended

Security Context

This project demonstrates least privilege access

Shows awareness of attack surface reduction

Highlights why controlling inbound traffic is critical in real environments
I documented the project and included screenshots

Why This Project Matters

Most cloud incidents do not start with advanced attacks. They start with misconfigured network access.

This project shows that I can:

Identify exposure

Apply least privilege network access

Test my controls

Explain security decisions

Outcome

By adding rule explanations, testing validation, and context, this project now demonstrates:

Practical NSG security implementation

Understanding of least privilege and attack surface reduction

Clear, tested, and explainable results.
