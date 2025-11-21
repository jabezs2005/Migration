# Migration
EX 6: MOVING FILES BETWEEN VIRTUAL MACHINES
NAME: GURU PRASATH R
REG NO: 212222040053
Aim:
To move the files between virtual machine. You can move files between virtual machines in several ways: • You can copy files using network utilities as you would between physical computers on your network. To do this between two virtual machine: • Both virtual machines must be configured to allow access to your network. • Any of the networking methods (host-only, bridged and NAT) are appropriate. • With host-only networking, you copy files from the virtual machines to the host and vice-versa, since host-only networking only allows the virtual machines see your host computer. • With bridged networking or NAT enabled, you can copy files across your network between the virtual machines. • You can create a shared drive, either a virtual disk or a raw partition, and mount the drive in each of the virtual machines.

Procedure:
How to Enable File sharing in VirtualBox.
Step 1. Install Guest Additions on the Guest machine. Step 2. Configure File Sharing on VirtualBox.

Step 1. Install Guest Additions on the Guest machine.

Start the Virtuabox Guest Machine (OS).
From Oracle's VM VirtualBox main menu, select Devices > Install Guest Additions *
a. Open Windows Explorer b. Double click at the "CD Drive (X:) VirtualBox Guest additions" to explore its contents.

<img width="776" height="622" alt="image" src="https://github.com/user-attachments/assets/ad1e9b5e-f0f0-4978-876d-92915b455660" />


C.Right click at "VBoxWindowsAdditions" application and from the pop-up menu, choose "Run as administrator".

<img width="1005" height="484" alt="image" src="https://github.com/user-attachments/assets/79b8963c-68fc-45ee-91e6-253f92a63d4c" />


3.Press Next and then follow the on screen instructions to complete the Guest Additions installation.

<img width="792" height="523" alt="image" src="https://github.com/user-attachments/assets/da55a29a-3e21-4384-91ca-5d0b57929a60" />

When the setup is completed, choose Finish and restart the Virtuabox guest machine. Step 2. Setup File Sharing on VirtualBox Guest Machine.
From VirtualBox menu click Devices and choose Shared Folders -> Shared Folder Settings.

<img width="905" height="530" alt="image" src="https://github.com/user-attachments/assets/69924ba2-d6ca-47fe-8a71-10566ffcd028" />


Click the Add new shared folder icon.

<img width="908" height="527" alt="image" src="https://github.com/user-attachments/assets/10fd3a70-9f74-4e25-9520-77e1b5c32e28" />


Click the drop-down arrow and select Other.

<img width="931" height="653" alt="image" src="https://github.com/user-attachments/assets/e970bddd-3526-41ca-a009-63dff85a9093" />


Locate and highlight (from the Host OS) the folder that you want to share between the VirtualBox Guest machine and the Host and click Select Folder. *
Note: To make your life easier, create a new folder for the file sharing, on the Host OS and give it with a recognizable name. (e.g. "Public")

<img width="880" height="448" alt="image" src="https://github.com/user-attachments/assets/fa16848c-c2f7-47f7-a3d0-52ea58bbbaad" />


Now, in the 'Add Share' options, type a name (if you want) at the 'Folder Name box, click the Auto Mount and the Make Permanent checkboxes and click OK twice to close the Shared Folder Settings.
image

<img width="925" height="461" alt="image" src="https://github.com/user-attachments/assets/b07b147d-fcf2-4c36-b54b-79537498c480" />

You 're done! To access the shared folder from the Guest OS, open Windows Explorer and under the 'Network locations' you should see a new network drive that corresponds to the shared folder on the Host OS.
Result:
Thus the virtual machine files are moved to another VM.
