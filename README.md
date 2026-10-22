# SporeWar: RotRising

SporeWar: RotRising is a top-down shooter developed using Unreal Engine 5.4.

This repository contains the game project and the files required to build it using Unreal Engine 5.4 and Visual Studio 2022.

## Prerequisites

Before setting up the project, make sure you have installed the following software.

### 1. Unreal Engine 5.4

Install Unreal Engine 5.4 through the Epic Games Launcher.

The project is designed to work with Unreal Engine 5.4. Using another engine version may cause compatibility issues.

### 2. Visual Studio 2022

Install Visual Studio 2022 with the components required for Unreal Engine C++ development.

During installation, select the following workload:

- Game development with C++

Make sure the required C++ compiler, Windows SDK, and other components needed for Unreal Engine development are installed.

If Visual Studio 2022 is already installed, open the Visual Studio Installer, select Modify, and verify that the required workload and components are installed.

### 3. Git

Install Git to clone the repository.

Alternatively, you can download the repository as a ZIP file from GitHub.

---

## Installation and Setup

Follow these steps in order to set up and compile the project.

### Step 1: Clone the Repository

Open a terminal in the directory where you want to store the project and run:

```bash
git clone <repository-url>
```

Replace `<repository-url>` with the URL of this GitHub repository.

Alternatively, open the repository on GitHub, click the green **Code** button, select **Download ZIP**, and extract the downloaded archive.

Once the repository has been downloaded, open the project folder.

### Step 2: Generate Visual Studio Project Files

Before opening the project in Visual Studio, generate the required solution and project files.

1. Open the folder containing the cloned repository.
2. Locate the Unreal Engine project file named `AlienShooter.uproject`.
3. **Right-click `AlienShooter.uproject`.**
4. If you are using Windows 11, select **Show more options** from the context menu.
5. In the expanded context menu, click **Generate Visual Studio project files**.
6. Wait for Unreal Engine to finish generating the files.

After the process completes, a Visual Studio solution file named `AlienShooter.sln` should appear in the project folder.

**Note:** If the Generate Visual Studio project files option is missing, verify that Unreal Engine 5.4 is installed correctly and that its project file associations are configured.

### Step 3: Open the Solution in Visual Studio 2022

1. Return to the root folder of the cloned repository.
2. Locate the generated file named `AlienShooter.sln`.
3. **Double-click `AlienShooter.sln`** to open it in Visual Studio 2022.
4. Wait for Visual Studio to finish loading the solution and its projects.

Make sure you open the `.sln` file rather than opening an individual C++ source file.

### Step 4: Set AlienShooter as the Startup Project

Once the solution has loaded, configure the correct startup project.

1. In Visual Studio, locate the **Solution Explorer** panel. It is usually on the right side of the window.
2. If Solution Explorer is not visible, open the **View** menu at the top of Visual Studio and click **Solution Explorer**.
3. In Solution Explorer, locate the project named `AlienShooter`.
4. **Right-click the `AlienShooter` project.**
5. Click **Set as Startup Project**.

The `AlienShooter` project should now be displayed in bold in Solution Explorer, indicating that it is the startup project.

**Important:** Make sure `AlienShooter` is selected as the single startup project before proceeding.

### Step 5: Select the Build Configuration

At the top of the Visual Studio window, locate the build configuration and platform dropdown menus.

Select the following settings:

- **Configuration:** Development Editor
- **Platform:** Win64

These settings are used to compile the project for the Unreal Editor on Windows.

If these options are not immediately visible, check the toolbar configuration or the available solution build configurations.

### Step 6: Compile the Project

Once the startup project and build configuration have been set, compile the solution.

1. At the top of Visual Studio, click the **Build** menu.
2. Select **Build Solution**.
3. Alternatively, press `Ctrl + Shift + B` on your keyboard.
4. Wait for Visual Studio to finish compiling the project.

You can monitor the progress in the Output window at the bottom of Visual Studio.

If the Output window is not visible, open the **View** menu and select **Output**.

Wait until the build finishes and check the output for compilation errors.

The initial build may take several minutes, depending on your hardware.

**Do not close Visual Studio while the project is compiling.**

### Step 7: Open the Project in Unreal Engine 5.4

After the compilation completes successfully:

1. Return to the folder containing the repository.
2. Locate `AlienShooter.uproject`.
3. **Double-click `AlienShooter.uproject`** to launch the project in Unreal Engine.
4. If Windows asks which Unreal Engine version to use, select Unreal Engine 5.4.
5. Wait for the editor to finish loading the project.

The first launch may take additional time while Unreal Engine compiles shaders and performs initial setup.

Once the editor has finished loading, the project is ready to use.

---

## Troubleshooting

### Generate Visual Studio Project Files Is Missing

If the option does not appear when right-clicking `AlienShooter.uproject`:

- Verify that Unreal Engine 5.4 is installed.
- Verify that Visual Studio 2022 is installed with the required C++ development tools.
- Check that the Unreal Engine project file associations are configured correctly.

### Compilation Errors in Visual Studio

If the project fails to compile:

- Verify that Unreal Engine 5.4 is installed.
- Confirm that the required Visual Studio C++ components and Windows SDK are installed.
- Make sure `AlienShooter` is set as the startup project.
- Confirm that the selected configuration is `Development Editor` and the platform is `Win64`.
- Review the Output window for the specific compilation error.

### Unreal Engine Cannot Open the Project

If the editor fails to open the project:

- Verify that the `.uproject` file exists in the repository folder.
- Confirm that the correct Unreal Engine version is installed.
- Check whether the initial compilation completed successfully.
- Review any error messages displayed by Unreal Engine.

---

## Technology Stack

- **Game Engine:** Unreal Engine 5.4
- **Programming Language:** C++
- **IDE:** Visual Studio 2022
- **Target Platform:** Windows PC

## Developer

**Inverted Button Studios**

Website: https://invertedbuttonstudios.com/

## Project Status

Released on Steam.

## License

Unless otherwise specified, the game's source code, artwork, and other project assets remain the property of their respective owners.

Please contact Inverted Button Studios for permission before redistributing or using proprietary project materials.
