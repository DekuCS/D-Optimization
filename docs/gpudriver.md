## 🚀 **Installing NVIDIA graphics drivers**

We recommend using NVCleanstall, as it is a GUI alternative to manually stripping drivers.

### ✅ Driver Installation
- Download NVCleanstall.
- Open the application and click Next.
- Make sure that only Display Driver is checked and click Next.
- After the driver downloaded tick the following:
  - Disable Installer Telemetry & Advertising
  - Perform a Clean Installation
  - Disable Multiplane Overlay (MPO)
  - Disable Driver Telemetry in Show Expert Tweaks
  - Use method compatible with Easy-Anti-Cheat
  - Automatically accept the "driver unsigned" warning
- Click **Install** and continue with the NVIDIA driver installation as usual.

### ⚙️ Configure NVIDIA Control Panel
- Open the NVIDIA Control Panel by right-clicking on dekstop.
- Disable `Desktop > Show Notification Tray Icon`
- Configure the following in the `3D Settings -> Manage 3D settings` page:
  - Anisotropic filtering - Off
  - Antialiasing - Gamma correction - Off
  - Low Latency Mode - On (This setting limits pre-rendered frames to 1)
  - Power management mode - Prefer maximum performance
  - Shader Cache Size - Unlimited
  - Texture filtering - Quality - High performance
  - Threaded Optimization - Offloads GPU-related processing tasks on the CPU, it usually hurts frame pacing. If you are CPU bottlenecked,     choose the `Off` option.
  - Vertical sync - Off
- Configure the following in the Display -> `Change resolution` page:
  - Configure your monitor resolution and refresh rate.
  - Output dynamic range - Full
  - Output color depth - Value matching your monitor specification
- Optionally increase the level of `Digital vibrance` in `Display -> Adjust desktop color settings` as it manages color saturation and        intestity, and can reduce eye strain. 
  - Also check out [VibranceGUI](https://vibrancegui.com/).
- Configure the following in the `Display -> Adjust desktop size and position` page:
  - Select a scaling mode - No scaling
  - Perform scaling on - Display
- Set dynamic range to `Full` in `Video -> Adjust video color settings -> Advanced`

- Now run [nvidiaProfileInspector](https://github.com/Orbmu2k/nvidiaProfileInspector) scroll down to `5 - Common section` and set `CUDA - Force P2 State` to OFF. Press `Apply changes` on the upper right corner and close the application. **Restart your device**.
