 ![image](https://github.com/user-attachments/assets/5d1f41a9-e3e7-4441-a67b-237c2c62df35)

<h1> Software & Driver Installation Troubleshooting in Office 365 </h1>
 <br /> This project involves creating a detailed documentation guide on installing, updating, and troubleshooting essential IT support software. I am going to use Microsoft 365. The guide will also walk through the process of handling common issues, demonstrating my troubleshooting and problem-solving skills.<br />


<h2>Environments and Technologies Used</h2>

- Windows 10

<h2> Software Choice </h2>

- Microsoft Office 365

<h2>List of Steps </h2>

- Install Microsoft Office 365
- Update Microsoft Office 365
- Troubleshooting Common Issues

<h2> Part 1 Installation and Upgrading Microsoft 365 </h2>
(Image 1)

<img width="959" alt="image" src="https://github.com/user-attachments/assets/bdb18f29-819f-41e4-9601-4f1fac575a65" />

(Image 2)

<img width="176" alt="image" src="https://github.com/user-attachments/assets/d9be34e7-c887-4489-aa98-18435ce1afd2" />

(Image 3)

![image](https://github.com/user-attachments/assets/beb6ccdc-aaab-468b-8074-6c57f01423c9)


#1. Downloading & Installing Office 365 - Sign in to Microsoft 365 Open a web browser and go to https://www.office.com. Click on "Sign in" and enter the Microsoft 365 account credentials provided by your organization or personal Microsoft account. Once signed in, click on "Install apps" in the upper right corner. Select "Microsoft 365 apps" to download the installation file. Once the file (Setup.exe on Windows or .pkg on macOS) is downloaded, locate it in your Downloads folder. Double-click the installer to begin the installation process. Follow the on-screen prompts: Accept the license agreement. Choose the installation location (default is recommended). Click "Install" to begin the process. Wait for the installation to complete. When finished, click "Close", and restart your computer if prompted. Open any Office app (e.g., Word, Excel, Outlook). A Sign-in prompt will appear. Enter the Microsoft 365 account credentials used during installation. If prompted, choose your organization’s settings (Work/School or Personal). Click "Activate", and Office will verify the license. Once activated, Office is ready to use.

(Image 1)

<img width="261" alt="image" src="https://github.com/user-attachments/assets/b46c44cb-c8f4-420e-8f25-327e155cf2b3" />


(Image 2)

<img width="240" alt="image" src="https://github.com/user-attachments/assets/d00fc7e2-2efd-4bdb-94ec-bd2e6d60890c" />


#2. Updating Microsoft Office 365 - Keeping Office 365 updated ensures you have the latest security patches and features. Open Office Update Settings. Open Microsoft Word (or any Office app). Click on "File" > "Account" (in some versions, it may be "Office Account"). Under Product Information, locate the Update Options button. Click "Update Options" > "Update Now". Office will check for updates and begin downloading them if available. If updates are installed, a message will confirm it: “You're up to date”. In the same Update Options menu, select "Enable Updates" to ensure Office updates automatically.

<h2> Part 2 Installation and Upgrading Netwrork Adapter </h2>


(Image 1)
<img width="958" alt="image" src="https://github.com/user-attachments/assets/40110ff2-a6e3-46a2-b9ce-72895e78db77" />

#1. Establishing Temporary Internet Access - Since the PC had no existing wireless capability, I connected it to the router using an Ethernet cable. This allowed me to access the Netgear support website to download the correct A6100 driver and software package directly from the source, ensuring compatibility and up-to-date files.


(Image 1)
<img width="952" alt="image" src="https://github.com/user-attachments/assets/170dfbb9-5aaa-446f-929d-a0a34c7fb24c" />


(Image 2)

<img width="760" alt="image" src="https://github.com/user-attachments/assets/b61cc2b8-2116-4503-ad1b-33e230b472c5" />


#2. Installing the Netgear A6100 Drivers - After downloading the driver package, I ran the installation executable and followed the guided setup. I unziped the Netgear A1600 files and downloaded the standalone file. Once installed, I safely removed the Ethernet connection and connected the Netgear A6100 USB WiFi adapter to an available USB port. Windows recognized the adapter, and the driver initialized the wireless connection module.


(Image 1)
<img width="266" alt="image" src="https://github.com/user-attachments/assets/db121d53-7101-41e4-801b-f9431b3ca253" />

(Image 2)

<img width="611" alt="image" src="https://github.com/user-attachments/assets/a7e106a2-7174-4928-b861-f756d83a6052" />


#3.  Connecting to a Wireless Network & Verifying Internet Connectivity via PowerShell - I opened the network settings, scanned for available WiFi networks, and connected the PC to my home network using the correct credentials. The system showed a successful connection with full signal strength, confirming the adapter was functioning properly. To confirm the connection, I launched PowerShell and ran the command:
ping www.google.com
Successful replies verified that the PC had active internet access through the Netgear A6100 adapter, completing the setup process.


<h2> Part 3 Troubleshooting Common Office 365 Issues </h2>

If Office 365 encounters problems, use the following troubleshooting methods:


Issue 1: Office Apps Not Opening or Crashing


<img width="958" alt="image" src="https://github.com/user-attachments/assets/c6901bac-911f-4e98-913f-a5548104b6f7" />


Fix: Restart the computer and try again. Open Task Manager (Ctrl + Shift + Esc), find any running Office processes, and end task.
Run Office in Safe Mode: Press Win + R, type winword /safe, and hit Enter.


Issue 2: Office 365 Activation Error

<img width="938" alt="image" src="https://github.com/user-attachments/assets/c8c07199-3df1-4bde-a580-22b4c8109b7b" />

<img width="611" alt="image" src="https://github.com/user-attachments/assets/b918b64a-4345-4673-8636-a2dbbf3e99ae" />

Fix: Sign out of Office and sign back in with the correct account. Check internet connectivity through powershell. Ping to the loopback address. ( ping 127.0.0.1 ) You can also check the firewall settings.
Go to File > Account > Update License and try again.


Issue 3: Office 365 Not Updating


<img width="261" alt="image" src="https://github.com/user-attachments/assets/b46c44cb-c8f4-420e-8f25-327e155cf2b3" />

Fix: Check if automatic updates are enabled (File > Account > Update Options > Enable Updates).
Run Office as an administrator and retry the update.
Manually download the latest update from Microsoft's Office website.


Issue 4: Slow Performance in Office Apps


<img width="581" alt="image" src="https://github.com/user-attachments/assets/0defa1eb-97b1-4b00-80e2-15892bc04ffa" />


<img width="220" alt="image" src="https://github.com/user-attachments/assets/dd6eb1cd-85ed-4447-a5d8-e991653eb392" />

Fix: Disable add-ins (File > Options > Add-ins > Manage COM Add-ins > Disable unnecessary add-ins).
Repair Office (Control Panel > Programs > Microsoft Office > Modify > Quick Repair).
Ensure the system meets Office requirements (RAM, storage).





