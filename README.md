# Download Azure VPN Client

To install Azure VPN Client using the EXE package, follow the steps below. For organization-wide deployments, you can utilize the `msiexec` command in the terminal to manage the installation process.

1. Get the appropriate version of the Azure VPN Client installer that matches your system.

2. Launch the installer by double-clicking the downloaded executable.

3. When the welcome screen appears, click **Next** to proceed.

4. Review the license agreement, check the box labeled **I accept the terms in the License Agreement**, and click **Next**.

5. In the Installation Scope section, choose one of the following:

* **Install only for you**: Installs the client to a user-specific folder, making it accessible solely from your user account. No admin rights are required.

* **Install for all users on this machine**: Makes the client available for all users on the computer. This option requires administrative privileges.

6. Click **Install** to start the installation.

7. Once the installation finishes, click **Finish**.

8. If the checkbox **Launch Azure VPN Client when setup exits** is enabled, the application will open automatically. Otherwise, you can manually launch it by searching for **Azure VPN Client** via the Start menu.

Before initiating a connection to your apps or devices on Windows, ensure the following prerequisites are met:

* An active internet connection
* One of the following supported Windows editions:

  * Windows 11
  * Windows 10
  * Windows Server 2022
  * Windows Server 2019
  * Windows Server 2016
* .NET Framework 4.6.2 or newer. On some builds of Windows 10 or Windows Server 2016, you may need to install it manually. Visit the official .NET Framework download page for the latest installer.

### .NET 8 requirement

Starting with version 4.0.1.0, the desktop edition of Azure VPN Client depends on the .NET 8 runtime. If it’s not already present, the MSI installer will download and install .NET 8 automatically. Without this runtime, systems must have access to the following URLs:

* [https://aka.ms/dotnet/8.0/windowsdesktop-runtime-win-x64.exe](https://aka.ms/dotnet/8.0/windowsdesktop-runtime-win-x64.exe)
* [https://aka.ms/dotnet/8.0/windowsdesktop-runtime-win-x86.exe](https://aka.ms/dotnet/8.0/windowsdesktop-runtime-win-x86.exe)

The client leverages the .NET 8 runtime to provide the most modern and responsive UI. Even on 64-bit systems, the 32-bit runtime is needed because certain internal automation features function exclusively in 32-bit mode.

If you encounter an error stating that the .NET 8 runtime installation has failed, it's likely due to connectivity issues or an incomplete package installation. To resolve this, manually install both runtime packages. Once installed, future versions of the Azure VPN Client will no longer attempt to download .NET 8.

### Android

To install the Azure VPN Client on Android devices, use one of the following app stores:

* [Portal AppStore](*)
* [Google Play](*)
* [Amazon Appstore for Android](*)

If these platforms are unavailable, or if your device lacks support for Google Mobile Services, you can [manually download Azure VPN Client for Android](*). Keep in mind that manually installed (sideloaded) apps won’t receive automatic updates or security patches — you’ll need to update them yourself.

In the People’s Republic of China, the Google Play Store is inaccessible. In this case, use a trusted Chinese app marketplace to install the app.

### iOS

To install Azure VPN Client on iOS, download it directly from the [Apple App Store](*).

### macOS

To install Azure VPN Client on macOS, visit [Enroll my Mac](*). This link automatically begins downloading the installation package to your Mac.

## Sign in to app

You can access the Azure VPN Client app using one of three authentication methods:

* Sign in using your school or work email and password.
* Use certificate-based authentication.
* Authenticate from another device.

For the smoothest experience, always follow the sign-in method preferred or required by your organization.

### Sign in with school or work account

1. Launch the app and click **Sign In**.
2. Provide your school or work email, then click **Next**.
3. Enter your password and click **Sign In**.
4. Wait while your credentials are validated. Once authenticated, you'll gain access to app features and your organization's resources.

### Sign in with certificate

This option will appear only if your organization supports authentication via certificate and a valid certificate is available.

1. Launch the Azure VPN Client app on your device.
2. Enter your associated school or work email and click **Next**.
3. Choose **Sign in with a certificate**.
4. Tap **Continue** to confirm the selected certificate.
5. The app will verify the certificate. Once approved, you'll be able to use the client and connect to your organization’s network.
