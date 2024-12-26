# Hackintosh Compatibility for Dell Vostro 15 3568

Here's a table summarizing the components of the Dell Vostro 15 3568 Hackintosh setup, including what works and what doesn’t.
| **Component**         | **Status**            | **Notes/Additional Information**       |
|-----------------------|-----------------------|----------------------------------------|
| **macOS Installation** | ✅ Works              | macOS Ventura, smooth installation. |
| **Wi-Fi**              | ✅ Works              | Fully functional, even when installing from USB (in recovery mode).  |
| **Bluetooth**          | ✅ Works              | Fully functional, connects to devices. |
| **Ethernet**           | ✅ Works              | Wired Ethernet connection works out of the box. |
| **Built-in Camera**    | ✅ Works              | Integrated camera is detected and works. |
| **Audio (Speakers)**   | ✅ Works              | Audio works without additional drivers. |
| **Audio (Headphones)** | ✅ Works              | Headphone jack is functional. Install Combojack. |
| **Battery**            | ✅ Works              | Battery status and sleep work properly. |
| **Trackpad**           | ✅ Works              | Trackpad is fully responsive, including gestures. |
| **Keyboard**           | ✅ Works              | Built-in keyboard works fine.          |
| **USB Ports**          | ✅ Works              | All USB ports (including USB 3.0) function correctly. |
| **iMessages / FaceTime**| ✅ Works             | Working after proper SMBIOS configuration. |
| **App Store**          | ✅ Works              | App Store works, can download apps.   |
| **Touchpad Gestures**  | ✅ Works              | Multi-finger gestures work well.      |
| **GPU**   | ✅ Works              | Intel HD 620 graphics are accelerated. |
| **Camera (FaceTime)**  | ✅ Works              | FaceTime camera is detected and works. |
| **Bluetooth Audio**    | ✅ Partially Works   | Works but if Device goes to sleep, needs to restart. |
| **Touch Screen**       | ❓ Not Supported      | - |

---
![398708598-e9ba5b6f-0f81-4eb5-a95c-a877cbf7a838 (1)](https://github.com/user-attachments/assets/1050187e-4a70-407d-9c9d-e353a94dd3ac)

## Notes:
- **Wi-Fi**: If you experience issues, reinstall the correct Intel Wi-Fi kexts (e.g., `IntelMausiEthernet.kext`).
- **Audio**: Ensure that all audio kexts are properly installed; check the `config.plist` for any missing settings if needed.
- **iMessages and App Store**: Make sure your **SMBIOS** is correctly configured in the `config.plist`. This is crucial for Apple services to work.
