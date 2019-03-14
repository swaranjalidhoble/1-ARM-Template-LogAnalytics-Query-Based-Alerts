# AzureLogAnalyticsAlerts
This ARM Template will help you to create Azure log analytics query based alerts for below resource providers and listed paramter alerts.

You should log analytics workspace created along with necessary solutions deployed (in this case only one solution is needed - AD Relication). You need have all rescources with below resource provider types connected to your log analytics worksapce.

You can create similar alerts for different resources as well by providing correct query, thresholds and triggers.

1. Azure VM

a. VM CPU
b. VM Memory
c. VM Disk
d. VM with Cleaned Event Log
e. VM with Guest logon
f. VM Restart
g. VM missing security Patches
h. VM shutdown
i. VM with detected threat

2. Azure Keyvault

a. Unauthorized user accessing keyvault

3. Virtual Machine Scale Sets

a. VMSS running node count below threshold
b. No VMSS nodes running

4. Operation Activity

a. Any Creation activity performed on subscription
b. Any Delection activity performed on subscription

5. Log Analytics Usage

a. Daily DataLimit Reached for LA is reached

6. Active Directory Replication

a. Source Server has errors in AD replication
b. Destination Server has errors in AD replication
c. Replication has issues

