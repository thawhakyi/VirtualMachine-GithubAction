# Free Virtual Machine by Github Action

Totally FREE for everyone to enjoy your own MacOS, Windows 10 and ubuntu vps.

## Screenshots:
<details>
    <summary>Windows 10</summary>
<br>
    
- Windows 10 Version
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/268600af-c8b9-47cf-b5dd-d1c1ed6d9ce9.png">

- Windows 10 Task Manager
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/0cf98258-a6fe-46bb-ac9a-ee4bb3037e3a.png" >

- Windows 10 Device Manager
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/d32cf285-5ecf-4cce-a52a-5cb54fb130c7.png">

- Windows 10 Device Specification
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/e1852b80-d550-44f3-b619-86ea82902bb4.png">
    
</details>

<details>
    <summary>Ubuntu (SSH Version)</summary>
<br>

1. Click **Run Workflox**
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/96644176-D760-47D4-BED2-C47E62A6763F.png" >

2. Copy ssh with url
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/0F804C5F-FE8F-45FA-9720-F91F212597DF.png" >

3. Open cmd or Terminal from your windows/MacOS or Linux, and type command provided by github actions boxes.
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/78FE6C5A-7270-4986-AB8F-57EC4C9B4F44.png" >

type **yes** from the connect, and then type your ssh password by secrets of LINUX_USER_PASSWORD u have set.

4. Type **sudo -i** for root permission and type your password.
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/E5527744-1ED1-4550-8867-EF4EC76D6895.png" >

5. Enjoy having your FREE linux SSH VPS and type any command you want.(but only 6 hours)
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/E6E9EA63-AC24-4FDB-AAF9-8B509658440A.png" >

</details>

<details>
    <summary>Ubuntu (Desktop Remote Version)</summary>
<br>

- Desktop Screenshot
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/4EB9C2FF-9D03-4998-A440-D7716A0F7CD0.png" >

- Linux Chrome
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/09F0A4CF-9B30-44CD-8DC4-139D03DFC2CC.png" >

- Install any apps you want :)
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/A0886141-DF1E-4379-88E7-F00EDAD87D0E.png">

</details>

<details>
    <summary>MacOS</summary>
<br>

- Desktop Screenshot
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.32.41%20AM.png" >

- Settings
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.32.21%20AM.png" >

- RAM
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.32.58%20AM.png" >

- Storage
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.33.18%20AM.png" >

- Pre-Installed Apps
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.34.10%20AM.png" >

</details>

## Machine Specification:
### Windows and Linux:
- 2-core vCPU
- 7 GB RAM
- 14 GB SSD Disk **(Excluded System used)**
### MacOS 10.15
- 3-core vCPU
- 14 GB RAM
- 14 GB SSD Disk **(Excluded System used)**

## Setting up:
1. Fork this project
2. Go to your peoject page, click `Settings` and go to `Secrets`, and then click `New Secret` to add these secrets below:

Secrets Name | Uses | Notes
----- | ----- | -----
`MAC_REALNAME` | For MacOS User Display Name | Type any name you want
`MAC_USER_PASSWORD` | For MacOS System Admin Password | Type any password you want
`NGROK_AUTH_TOKEN` | For **ngrok** tunnel uses | Go to website, and copy the API key from https://dashboard.ngrok.com/auth/your-authtoken
`VNC_PASSWORD` | For the login password of VNC remote authentication | Type any password you want
`WINDOWS_USER_PASSWORD` | For Windows 10 RDP login password | Type any password you want
`LINUX_USERNAME` | For linux system username | Type any name you want
`LINUX_USER_PASSWORD` | For linux shell and root password | Type any password you want
`LINUX_MACHINE_NAME` | For Linux System Computer name | Type any name you want
`CHROME_HEADLESS_CODE` | For remoting linux desktop using google remote | Copy Codes from [here](https://remotedesktop.google.com/headless) and login with your google account, and then copy the code below `Debian Linux` blank. :warning: Each code can only be used for once, generate another code when u have used that one.

## Deloy and Run
<details>
    <summary>MacOS Install and Run</summary>
<br>
    
1. go to `Actions` Tab and select one of system workflow.

2. Click `Run Workflow` button on the left of `This workflow has a workflow_dispatch event trigger` line.

3. Wait until a few minutes.

4. Go to https://dashboard.ngrok.com/status/tunnels and check if theres a one online tunnel running.

5. Copy the link(**without tcp://**) and go to VNC Viewer(Download and install it), input the link to connect area u copied from the website.

6. Fill in those login info, within username `koolisw`and password from `VNC_PASSWORD` you typed.

7. Enjoy!

</details>

- Reminders:
:warning: Dont close this windows which called "**provisioner.exe**", it will cause the windows system process to be stopped and disconnect from Windows RDP.
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/9a56f43b-0734-4186-b619-1588c208eb05.png">

:warning: Dont install big sur updates on your macos virtual machine, it will break your remote process!
<img src="https://raw.githubusercontent.com/thawhakyi/VirtualMachine-GithubAction/main/screenshots/Screenshot%202021-02-23%20at%207.35.57%20AM.png">

## Limits: 
1. You can run each virtual machine only run up for **6** hours for execution time. If Virtual Machine reaches this limit, it will be terminated and clear everything.
2. Not suggested for you saving some of important and sensitive files to each machine, be risked that all files will be deleted and cannot be undo.
3. Since we are using **ngrok**, you can only run one of those **three** system by one due to ngrok free plan limits, you cannot access both system at the same time unless you purchased **ngrok** pro or business plan.
4. Not suggested to login any account from any website (just like **Google or Microsoft**), since **VNC** connection is not encrypted and easily been accessed other people.

## Suggestions and Best Tricks:
- If you are facing slow and laggy remote control experience from **MacOS** or **Windows**, you can use either **Google Remote Desktop** or **Microsoft Remote Control** for a faster and smoother remotes.
- We highly recommanded you **fork** this project to change username and other displaying names for systems.
