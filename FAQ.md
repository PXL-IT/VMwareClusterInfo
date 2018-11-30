# FAQ

## Q1: What's the routable network?
**A1:** Every project has its own routable network. There is already one device up and running, which lives outside of your
VMware project. That device is the gateway, it will route traffic.

## Q2: We don't get an IP on our routable network via DHCP.
**A2:** Correct, there is no DHCP server on the routable network. The gateway, which is already there, only provides routing. Therefore, all servers should have a static IP address.
You received the project range via mail together with the login.

## Q3: The other networks don't have internet access.
**A3:** Correct, you have to setup your own routing towards the routable network.

## Q4: How can I create a new VM?
**A3:** There are two ways to create a new VM. The preferred manner is to create a VM from an existing template. There are a few templates available. You can view them in the second tab (VMs and Templates). There should be a folder called `Templates`. Just right click on the preferred template and `New VM from this Template...`.

The second way to create a VM is from scratch with an ISO. The ISO files can be found on each of the three `Local  compute datastores` under the directory `isos`. When you create a new VM, select at step `7 Customize hardware` under `New CD/DVD Drive *` the option `datastore ISO file`. Note: only the datastore where the VM will be made is accessable in this window. (We don't want to install a VM using an ISO file located on an other Compute node now, do we?). Select the ISO file of your choosing. **Do not forget to check `☑ Connect At Power On` before continuing to step 8!!!**

## Q4: Where can I find the ISO files to install a new Virtual Machine?
**A4:** The ISO files can be found on each of the three `Local  compute datastores` under the directory `isos`.

## Q5: Can we have a real public IP address?
**A5:** Yes, **but...** This will be evaluated from case to case. We need to know **why** and **which services and ports**. Only if the team can provide us with convincing evidence the serverices will be secure, an public IP will be granted.

## Q6: How can we communicate with Tim?
**A6:** I'll be as much as possible available on *Skype for Business* during the IT-Project hours. Login with your `student-number-mail-address` and search for my full name.

### Before the winter break:
IRL @ iSpace: Each afternoon of the IT Project. From around or a little bit after 14h00 until the end.

On Thursday the 20th and Friday the 21th of December, I won't be present at iSpace due to the opening of DronePort (the  manned and unmanned aviation campus and incubator).

### After the winter break:
At this moment it's still a little bit unclear when I'll be at iSpace and when at DronePort.
So, it's still: **TBA**.

## Q7: The AON and SWM students can't login via VPN.
**A7:** By default, PXL students don't have VPN access. You, SNB student, we're probably granted access for the Research Project during the previous academic year. I'm going to send a request to the PXL IT department to grant all students following the IT Project course VPN access. During the second week of the IT-Project, everyone should have VPN access. **If not, contact me!**


## Q8: What are the credentials of the templates?
**A8:** For the `-base-` templates it's: Login: `user`, password: `user`. Why so unsecure? To trigger you to change it **immediately**!