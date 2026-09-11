# AppTrace

**AppTrace** is a C# WPF desktop process inspector designed for real-time diagnostic monitoring, process analysis, and system activity inspection on Windows.

It provides deep visibility into running applications, allowing developers, security researchers, and power users to inspect what executables are doing under the hood.

---

## Key Features

* **Live Process Inspector:** Target and attach to any active Windows process from a live dropdown list.
* **Real-Time Telemetry:** Continuous tracking of Working Set memory usage (MB) and active system thread counts via background polling timers.
* **Loaded Module Enumeration:** Deep inspection of all `.dll` libraries and dependencies loaded into the target process's memory space.
* **Child & Parent Tree Detection:** WMI-powered discovery of helper and sub-processes spawned by the target application.
* **Network Socket Monitoring:** Live tracking of active TCP/UDP socket connections, local/remote IP addresses, and communication ports.
* **Force-Terminate Controls:** Forcefully kill unresponsive or frozen background process trees directly from the dashboard.
* **UAC Admin Elevation Guard:** Automatic administrator privilege detection and restart prompts to ensure access to protected system processes.
* **Custom Alert Dialogs:** Integrated `ErrorWindow` modal system for cleanly displaying access violations and privilege issues.
* **Exportable Diagnostic Reports:** One-click exporting of detailed inspection snapshots and activity logs to formatted text files.

---

## System Requirements & Architecture

* **Operating System:** Windows 10 / Windows 11 (64-bit)
* **Architecture:** `win-x64`
* **Framework:** .NET 8.0 / .NET 9.0 WPF
* **UI Controls:** `HandyControl` (Dark Mode Theme)
* **Dependencies:** `System.Management` (WMI integration)

---

## Getting Started

1. Download the latest standalone binary (**`AppTrace_winx64.exe`**) from the [Releases](../../releases) tab.
2. Run **`AppTrace_winx64.exe`**. If prompted, allow Administrator privileges to enable deep inspection of elevated processes.
3. Select a running process from the top dropdown menu and click **Attach Trace**.
4. Navigate through the tabs to inspect loaded modules, executable launch arguments, network activity, and activity logs.

---

## License

Distributed under the MIT License. See `LICENSE` for details.
