#To enable disk UUID on a virtual machine

You must set the disk.EnableUUID parameter for each VM to "TRUE". This step is necessary so that the VMDK always presents a consistent UUID to the VM, thus allowing the disk to be mounted properly. For each of the virtual machine nodes (VMs) that will be participating in the cluster, follow the steps below from the vSphere client:

## To enable dis UUID on a VM
 1. Power off the guest.
 2. Select the guest and select Edit Settings.
 3. Select the Options tab on top.
 4. Select General under the Advanced section.
 5. Select the Configuration Parameters... on right hand side.
 6. Check to see if the parameter disk.EnableUUID is set, if it is there then make sure it is set to TRUE.
    If the parameter is not there, select Add Row and add it.

 7 . Power on the guest.
