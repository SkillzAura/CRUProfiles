# 🖥️ CRU Profiles

A collection of optimized **Custom Resolution Utility (CRU)** profiles for specific monitors. These profiles focus on "debloating" display settings, removing ghost resolutions, and ensuring native compatibility without the clutter.

---

## 🎯 Purpose
Windows often populates your display settings with redundant resolutions and TV-standard timings (like 4K resolutions on 1080p panels) that can mess with GPU scaling and desktop behavior. These profiles provide a clean configuration by:

* **Removing Ghost Resolutions:** Stripping away virtual or redundant resolutions you don't use.
* **Fixing GPU Scaling:** Ensuring the GPU only scales based on the monitor's native specs.
* **Cleaning EDID Metadata:** Removing unnecessary extension blocks and "junk" data from the display driver.
* **Forcing Native Refresh Rates:** Ensuring Windows defaults to your monitor's highest rated speed.

---

## 📂 Repository Structure
Profiles are organized by manufacturer and model:

```text
/Profiles
  /ASUS
    /VG248QE.bin
  /BenQ
    /XL2411K.bin
  /ZOWIE
    /XL2546K.bin


## 🛠️ Installation Instructions
1.  **Download:** Grab the `.bin` or `.dat` file for your specific monitor model.
2.  **Open CRU:** Run `CRU.exe` (Custom Resolution Utility by ToastyX).
3.  **Import:** Click the **Import** button at the bottom and select the file you downloaded.
4.  **Save:** Click **OK** to close CRU.
5.  **Restart Driver:** Run `restart.exe` (or `restart64.exe`) found in the CRU folder. 
    * *Note: Your screen will flicker for a moment; this is normal.*
6.  **Verify:** Check your Windows Display Settings to ensure only the optimized resolutions remain.

## ⚠️ Important Disclaimer
> **Use at your own risk.** While these profiles are tested, every panel is slightly different. If your screen stays black after running `restart.exe`, wait 15 seconds for a revert or press **F8** to enter Safe Mode and run `reset-all.exe` from the CRU folder.

❓ FAQ

Q: Will this increase my FPS? A: No. This is for display cleanliness and proper scaling behavior, not for boosting raw frame rates.

Q: Do I need to re-apply this after a GPU driver update? A: Yes. Most driver updates (especially "Clean Installs") will reset your monitor's EDID override. Keep your .bin file handy.

🤝 Contributing
If you have a perfected profile for a specific monitor that isn't listed here, feel free to open a Pull Request! Please include:

Monitor Model Name

Main changes made (e.g., "Removed 4K virtual resolutions on a 1080p panel")

Specific Rev/Version (if applicable)
