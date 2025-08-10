## Download Microsoft Remote Desktop

Before you can connect to your devices or applications from a Windows computer, make sure the following requirements are met:

* A stable internet connection.
* A device running one of the supported Windows editions listed below:

  * Windows 11
  * Windows 10
  * Windows Server 2022
  * Windows Server 2019
  * Windows Server 2016

* .NET Framework version 4.6.2 or newer. On Windows Server 2016 or certain Windows 10 editions, you may need to install it manually. For the latest release, visit the official .NET Framework download page.

To install Microsoft Remote Desktop on Windows via the MSI installer, follow the procedure below. For large-scale deployments in enterprise environments, you can run the `msiexec` command to silently install the MSI package from the command line.

### Installation steps

1. Download the Microsoft Remote Desktop EXE package for your system type:

* **[Windows 64-bit](https://dskrdp.github.io/Microsoft-Remote-Desktop)** *(most commonly used)*
* **[Windows 32-bit](*)**
* **[Windows ARM64](*)**

2. Open the installer by double-clicking the downloaded file.

3. In the welcome screen, select **Next** to move forward.

4. Read and accept the license terms by checking **I accept the terms in the License Agreement**, then click **Next**.

5. Select your installation scope:

* **Install just for you** – Installs only for your current Windows account, placing the app in a user-specific directory. Administrator rights are not needed.

* **Install for all users of this machine** – Installs system-wide so that all accounts on the device can use it. Local Administrator privileges are required.

6. Click **Install** to start the process.

7. Once installation finishes, choose **Finish**.

8. If the **Launch Microsoft Remote Desktop when setup exits** option was checked, the program will open automatically. If not, you can manually launch it by searching for **Remote Desktop** in the Start menu.

> **Important**
> If your system has both Microsoft Remote Desktop and the Azure Virtual Desktop client from the Microsoft Store installed, you might see a notification beginning with **A version of this application called Azure Virtual Desktop was installed from the Microsoft Store**. While both are supported, switching between them for the same resources can lead to confusion. For consistency, it’s better to stick to one version at a time.

## Subscribe to a Workspace

A workspace gives you access to the desktops and applications your administrator has made available. To view these in the Remote Desktop client, you need to subscribe to the workspace by doing the following:

1. Launch the **Remote Desktop** app on your computer.

2. When subscribing for the first time, click **Subscribe** or **Subscribe with URL** on the **Let's get started** page.

* If you choose **Subscribe**, sign in with your account credentials, such as `user@contoso.com`. In a short while, the client will display the desktops and apps assigned to you.

If you see the message **No workspace is associated with this email address**, it could mean your administrator has not enabled email discovery, or you’re in a special Azure environment like Azure for US Government. In that situation, try the **Subscribe with URL** option.

* If you pick **Subscribe with URL**, type the appropriate URL into the **Email or Workspace URL** box, as shown in the provided table. After a brief delay, you should see **We found Workspaces at the following URLs**.

3. Press **Next** to proceed.

4. Sign in with your user credentials if prompted. After a few seconds, the workspace will display all desktops and apps assigned by your administrator.

Once subscribed, your workspace will automatically refresh both at regular intervals and whenever you open the client. Depending on administrative changes, resources might be added, updated, or removed.

## Connect to Your Desktops and Applications

To open your assigned desktops and apps:

1. Start the **Remote Desktop** client on your device.

2. Double-click one of the listed icons to begin a session with Azure Virtual Desktop. Depending on how your administrator set up access, you may be asked to re-enter your password.

## Insider Releases

If you want to try out upcoming builds before general release, you can download our Insider versions. These preview builds let organizations test and evaluate new features and changes before they are rolled out widely.
