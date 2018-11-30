# FAQ

## Q1: What's the routable network?
**A1:** Every project has its own routable network. There is already one device up and running, which lives outside of your
VMware project. That devices is the gateway, it will route traffic.

## Q2: We don't get an IP on our routable network via DHCP.
**A2:** Correct, there is no DHCP server on the routable network. The gateway, which is already there, only provides routing. Therefore, all servers should have a static IP address.
You received the range via mail with together with the login.

## Q3: The other networks don't have internet access.
**A3:** Correct, you have to setup your own routing towards the routable network.

## Q4: How can I create a new VM?
**A3:** There are two ways to create a new VM. The preferred manner is to create a VM from an existing template. There are a few templates available. You can view them in the second tab (VMs and Templates). There should be a folder called `Templates`. Just right click on the preferred template and `New VM from this Template...`.

The second way to create a VM is from scratch with an ISO. The ISO files can be found on each of the three `Local  compute datastores` under the directory `isos`. When you create a new VM, select at step `7 Customize hardware` under `New CD/DVD Drive *` the option `datastore ISO file`. Note: only the datastore where the VM will be made is accessable in this window. (We don't want to install a VM using an ISO file located on an other Compute node now, do we?). Select the ISO file of your choosing. **Do not forget to check `☑ Connect At Power On` before continuing to step 8!!!**

## Q4: Where can I find the ISO files to install a new Virtual Machine?
**A4:** The ISO files can be found on each of the three `Local  compute datastores` under the directory `isos`.

## Q5: Can we have a real public IP address?
**A5:** Yes, **but...** This will be evaluated from case to case. We need to know **why** and **which services and ports**. Only if the team can provide us with convincing evidence the serverices will be secure, an public IP will be granted.