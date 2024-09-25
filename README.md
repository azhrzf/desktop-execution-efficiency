# Desktop Execution Application Efficiency Tracker

## Overview

The **Desktop Execution Application Efficiency Tracker** is a powerful tool designed to monitor and test the efficiency of desktop applications while they are running. It provides valuable insights into various performance metrics, including:

- **CPU Usage**
- **Physical Memory Usage**
- **Virtual Memory Usage**
- **Bandwidth Sent**
- **Bandwidth Received**
- **Disk I/O Statistics**

Users can export the captured data into CSV format for further analysis or reporting.

## Why WinForms Integration is Required

The conversion of the application to a WinForms project is essential to facilitate seamless integration with other desktop applications. While WPF (Windows Presentation Foundation) offers powerful capabilities for building modern user interfaces, many legacy and third-party applications are built on WinForms. By using WinForms, our application can leverage the following benefits:

- **Interoperability**: WinForms provides better support for integrating with existing WinForms applications and controls, allowing for easier communication and data exchange between different software components.

- **Accessibility**: Many organizations still utilize legacy WinForms applications; converting to WinForms ensures that our application can be incorporated into these environments without requiring extensive modifications to existing systems.

- **Simplified Deployment**: WinForms applications tend to have simpler deployment processes, making it easier to distribute and maintain the application within an organization.

- **Enhanced User Experience**: The integration of WPF User Control Libraries into WinForms allows developers to take advantage of modern UI features while still maintaining compatibility with traditional WinForms controls.

This hybrid approach enables us to harness the strengths of both WPF and WinForms, ensuring that our application remains flexible, efficient, and compatible with a wide range of desktop environments.


## Project Structure

The project consists of two main components:

- **WindowsFormsApp1**: This is the WinForms project that integrates the WPF User Control Library for monitoring desktop applications.
- **WpfControlLibrary1**: This is the WPF User Control Library containing the custom user controls used within the WinForms application.

## Features

- Real-time tracking of application performance metrics.
- Data export functionality to CSV format for easy analysis.
- Seamless integration of WPF controls within a WinForms application.
- Intuitive user interface for tracking and visualizing application performance.

## Installation

### Prerequisites

Ensure you have the following installed:

- [Visual Studio](https://visualstudio.microsoft.com/) (2019 or later recommended)
- .NET Framework (appropriate version for your project)

### Cloning the Repository

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/DesktopApplicationEfficiencyTracker.git
   ```
2. Open the solution file DesktopApplicationEfficiencyTracker.sln in Visual Studio.

### Adding the WPF Control Library to the WinForms Project
1. In Visual Studio, right-click on the WindowsFormsApp1 project in the Solution Explorer.
2. Select Add > Existing Project.
3. Navigate to the folder containing WpfControlLibrary1.csproj and select it.
4. Click OK.

### Integrating WPF User Control
1. Open the Toolbox in Visual Studio.
2. Expand WPF Interoperability and drag the ElementHost control onto your WinForms form.
3. Select the ElementHost control and set the hosted element:
4. Select Hosted Element > WpfControlLibrary1 > UserControl1.
5. Dock the ElementHost in the desired location on your WinForms form.

### Troubleshooting
If the UserControl does not appear:
1. Build and Clean the Solution:
    - Go to Build > Clean Solution.
    - Then select Build > Rebuild Solution.
2. Missing References or Packages: Ensure that the following references are included in your project:
    - DotNetProjects.DataVisualization.Toolkit
    - Microsoft.CSharp
    - PresentationCore
    - PresentationFramework
    - System
    - System.Core
    - System.Data
    - System.Data.DataSetExtensions
    - System.Diagnostics.PerformanceCounter
    - System.Drawing.Common
    - System.Management
    - System.Net.Http
    - System.Reactive
    - System.Reactive.Windows.Forms
    - System.Runtime.CompilerServices.Unsafe
    - System.Threading.Tasks.Extensions
    - System.Windows
    - System.Windows.Forms
    - System.Windows.Forms.DataVisualization
    - System.Xaml
    - System.Xml
    - System.Xml.Linq
    - WindowsBase
    - WindowsFormsIntegration
3. NuGet Packages: Make sure the following NuGet packages are installed:
    - DotNetProjects.WpfToolkit.DataVisualization
    - System.Diagnostics.PerformanceCounter
    - System.Drawing.Common
    - System.Reactive
    - System.Reactive.Windows.Forms
    - System.Runtime.CompilerServices.Unsafe
    - System.Threading.Tasks.Extensions

### Note
It is recommended to keep the WpfControlLibrary1 folder under the same parent directory as your WinForms project folder for easier management and reference.

### Usage
1. After setting up the project, run the WindowsFormsApp1 application.
2. The user interface will allow you to start monitoring the desired desktop application.
3. View the real-time performance metrics on the provided controls.
4. Use the export functionality to save the collected data in CSV format.
