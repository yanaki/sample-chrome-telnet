samples-chrome-telnet
======================

This sample shows how to develop a to-do hybrid mobile app using Google Chrome APIs in Telerik AppBuilder. You can clone this sample in Telerik AppBuilder, explore and modify the code, and build and run it on Android or iOS devices.

This sample demonstrates how to use the Socket API to connect as a TCP client to aardmud.org on port 4000

## Telerik AppBuilder and Chrome APIs

Google provides an Apache Cordova-based toolchain that lets developers wrap a Chrome App in a native container to make it available for Android and iOS devices. For a list of the Chrome Apps APIs that are currently supported for mobile development, click <a href="https://github.com/MobileChromeApps/mobile-chrome-apps/blob/master/docs/APIStatus.md" target="_blank">here</a>. 

> Google provides each API as a custom Apache Cordova plugin that you can import in Telerik AppBuilder. For more information about how to work with custom Apache Cordova in Telerik AppBuilder, click <a href="http://docs.telerik.com/platform/appbuilder/creating-your-project/using-plugins/using-custom-plugins/using-custom-plugins" target="_blank">here</a>.

Each Chrome API might depend on another Chrome API or a core Apache Cordova plugin. Telerik AppBuilder automatically resolves Apache Cordova core plugins dependencies but cannot resolve Chrome APIs dependencies. When you develop apps with Chrome APIs and Telerik AppBuilder, always make sure to import all interdependent Chrome APIs. The `plugin.xml` for the Chrome API lists all dependencies. 

## Sample Overview

The Telerik AppBuilder team has modified the existing Chrome telnet mobile sample to make it compatible with Telerik AppBuilder. You can find the source Chrome telnet mobile sample <a href="https://github.com/jordanilchev/samples-chrome-telnet/tree/master/samples-chrome-telnet" target="_blank">here</a>. 

The sample is initialized as a Chrome app. For more information about the development of Chrome apps, including the app container, click <a href="https://developer.chrome.com/apps/first_app" target="_blank">here</a>. 

All required Chrome APIs, including mobile and desktop APIs on which the app relies, are added as custom plugins.

The sample shows how to use the following methods and objects of the mobile Google Chrome APIs.

* **Socket API:**&nbsp;Lets you send and receive data over the network using TCP and UDP connections
* **Runtime:**&nbsp;Lets you manage the app lifecycle
* **Window:**&nbsp;Lets you create windows

## Cloning the Sample

You can clone this sample in Telerik AppBuilder, explore and modify the code, and build and run it on Android or iOS devices.

### Clone the sample in the in-browser client

1. Log in the Telerik Platform at <a href="https://platform.telerik.com" target="_blank">https://platform.telerik.com</a>.
1. Navigate to the workspace in which you want to clone the sample.
1. Click **Create project** and select **AppBuilder**.
1. Select **Clone repository**.
1. In the **Repository Uri** text box, paste `https://github.com/jordanilchev/samples-chrome-telnet.git`.
1. Provide a project name.
1. (Optional) Provide a project description.
1. Click **Create project**.

### Clone the sample in the Windows client

1. Run the Windows client and log in.
1. In the **Dashboard**, click **Clone**.
1. From the **Workspace** drop-down list, select the workspace in which you want to clone the sample.
1. In the **Repository Uri** text box, paste `https://github.com/jordanilchev/samples-chrome-telnet.git`.
1. Provide a project name.
1. Click **Clone**.

### Clone the sample in the extension for Visual Studio

1. In your browser, navigate to <a href="https://github.com/jordanilchev/samples-chrome-telnet" target="_blank">https://github.com/jordanilchev/samples-chrome-telnet</a>.
1. Click **Download ZIP**, store the archive on your local file system and extract it.
1. In {{ms-vs}}, create a new project from the *Blank* template.
1. In the **Solution Explorer**, select the `css`, `img`, `js`, and `App_Resources` folders, and the `index.html` file.
1. Press `Delete` and confirm that you want to delete the selected files and folders.
1. In Windows Explorer, go to the folder where you extracted the sample app and navigate to the subfolder that contains `index.html`.
1. Select all files and folders except `*.proj` and `cordova.*.js`.
1. Drag the selection to the **Solution Explorer** in {{ms-vs}} and drop it on your project node.
1. If prompted, confirm that you want to replace the existing files.

### Clone the sample in the command-line interface

1. In your browser, navigate to <a href="https://github.com/jordanilchev/samples-chrome-telnet" target="_blank">https://github.com/jordanilchev/samples-chrome-telnet</a>.
1. Click **Download ZIP**, store the archive on your local file system and extract it.
1. Run a command prompt, log in, and navigate to the folder that contains the `PROJ` file for the sample app.
1. Run `$ appbuilder init`.

The command-line interface shows the following message: `Successfully initialized project in the folder!`

## Running the Sample on Device

You can run this sample on iOS 7.0 and later devices and Android 4.0 and later devices. You cannot run this sample in the Telerik AppBuilder companion apps or the Telerik AppBuilder device simulator.

With Telerik AppBuilder, you can deploy apps on device wirelessly or via cable connection. For more information about running apps on devices, click <a href="http://docs.telerik.com/platform/appbuilder/testing-your-app/running-on-devices/working-with-devices" target="_blank">here.</a>

## License

[Liscence](License.md)
