# WinUI-Analog-Clock-UI

This repository contains a compact, self-contained WinUI-based analog clock user interface implemented as a sample desktop application.

Overview
---------
`WinUI-Analog-Clock-UI` demonstrates building a modern, analog clock using WinUI and .NET. The project focuses on clean XAML layout, vector assets, and time-driven rendering so the clock remains visually sharp across DPI settings and window sizes.

Key Features
------------
- Crisp vector-based clock face and hands that scale smoothly with window size and DPI.
- Smooth, time-accurate hand movement driven by a background timer.
- Simple asset structure under the `Assets/` folder for easy replacement of icons, backgrounds, and face elements.
- Minimal, easy-to-follow XAML and code-behind in `MainWindow.xaml` and `MainWindow.xaml.cs` so developers can adapt the UI quickly.

Requirements
------------
- Windows 10 (version 19041 or later) or Windows 11.
- .NET 6 SDK (or matching target framework used by the project).
- Visual Studio 2022 or later with the Universal Windows Platform / WinUI workload recommended for development and debugging.

Syncfusion WinUI RadialGauge
----------------------------
This sample uses the Syncfusion WinUI radial gauge control (`SfRadialGauge`) to render the clock face and hands. The gauge is referenced in `MainWindow.xaml` via the `Syncfusion.UI.Xaml.Gauges` namespace and provides the `SfRadialGauge`, `RadialAxis`, and `NeedlePointer` primitives used by the UI.

To build this project, add the Syncfusion WinUI Gauges package to the project via NuGet (or your preferred package manager) and ensure any required Syncfusion runtime registration or license steps are completed. Syncfusion controls are provided under Syncfusion's licensing terms — for evaluation or free community use, consult Syncfusion's website for details and registration instructions.

Build and Run
-------------
1. Open the solution in Visual Studio: open `AnalogClockUI.sln`.
2. Restore NuGet packages (Visual Studio typically does this automatically).
3. Build the solution and run using the debugger or run `dotnet build` from the solution folder and then launch the generated executable for the `net6.0-windows` target.

Customization
-------------
Replace vector assets in the `Assets/` folder to change the appearance of the clock face or hands. Adjust rendering and timing logic in `MainWindow.xaml.cs` if you need different behavior (for example, ticking vs. smooth sweep).

Contributing
------------
Contributions are welcome: open an issue to discuss changes or submit a pull request. Keep changes focused and provide a short description of the intent and testing steps.

License
-------
This sample is provided as-is for learning and demonstration purposes. Check the repository root for an explicit license file if one is included.

If you want, I can also add screenshots, CI build steps, or a packaged release workflow next.