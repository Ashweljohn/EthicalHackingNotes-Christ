Day 02

Installing Kali Linux on Oracle VirtualBox:

There are primarily 3 things Needed to install Kali linux on a Windows Host Machine.
1. Downloading Kali linux VirtualBox Image.(https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-virtualbox-amd64.7z)
2. Downloading 'Oracle VirtualBox'. It is a general-purpose full virtualization software.(https://download.virtualbox.org/virtualbox/7.1.12/VirtualBox-7.1.12-169651-Win.exe)
3. Downloading '7Zip'. It is a free and open-source file archiver with a high compression ratio. We are gonna use this for extracting the downloaded zip file.(https://www.7-zip.org/a/7z2500-x64.exe)

Note: Ensure you Have a minimum of 10-15 Gbs of Space in your Storage.

Step 1:
Installing Oracle VirtualBox on Windows host Machine.
1. Execute the downloaded VirtualBox installer.
2. Click on 'Yes' to provide the Administrator privilages needed.
3. Once Installer Dialogue box pops up click on 'Next'.
4. 'Custom Setup' page arrives. I suggest you don't do anything and press on 'Next'.
At the bottom left corner of the dialogue box defines the place where the software is gonna be installed.
5. Next "Warning! Network Interface' Page appears. Press 'Yes' to Continue.
6. Next "Missing Dependencies" Pages appears. Press 'Yes' to continue.
7. Next "Ready to install" Pages appears. Press 'Install'.
8. Click on 'Finish' and The VirtualBox is installed in your Host Machine.

TrobbleShooting Problems Occured during and after The installation of Oracle VirtualBox:
Problem 1
Missing 'Microsoft Visual C++ 2015-2022 Redistributable (x64) - 14.44.35211'
1. Click on the link to Download The dependency. https://aka.ms/vs/17/release/vc_redist.x64.exe and Install it.
2. Relauch the Oracle VirtualBox installer and Follow step 1.

 Problem 2
 AMD-V is diasabled in the BIOS(or by the Host OS)
1. Reboot Your System into Bios.
    To Enter into BIOS ,Check Your device model and Google for bios Key for that     Model. BIOS Key for some of the Famous Laptop's are Mentioned below.
      Dell: F2 or F12
Lenovo: F2 or Fn + F2 (for laptops), F1 (for desktops and all-in-ones), or the       Novo button
      Acer: F2 or DEL
      HP: Esc or F10
2. Navigate to Advance Setting Menu and search for Virtualization or SVM mode and Enable it.
    

Step 2:
Installing 7Zip tool.
1.Right click on downloaded 7Zip installer and "Run as Administrator".
2.An installer Diaglogue box appears, Click on 'Install'.
3.Click on 'Close' after installation.

Step 3:
Extracting the Downloaded Kali Linux VirtualBox Image Zip File.
1.Navigate to Directory where You have Downloaded the Kali Linux VirtualBox Image Zip file.
2.Right click on the Zip file and click on 'Show more options'. Move Your Cursor close to the 7Zip option and click on 'Extract here'.
3. It will take some time extracting the File after that the Extracting Taskj is Complete.

Step 4:
Loading the Kali Linux VirtualBox image File.
1.It is Advised to Create a Seperate pertetion in your Disk drive for Storing Kali linux.(10-15 Gbs would be sufficient)(https://www.youtube.com/watch?v=HGqo17dGk0E)
2.Copy the Extracted Kali Linux VirtualBox image File to the new partetion.
3. Open the folder and you will get 2 file types, 1.VirtualBox Machine Defination and 2.Virtual Disk Image File.Du need to double click on 'VirtualBox Machine Defination' Type file.
4. Oracle VirtualBox gets opened, Click on 'Start' to Turn on the Virtual Machine.Its going to take a when u are booting it for the First time.
5. After sucessful booting, Enter Username and password as 'kali'.
