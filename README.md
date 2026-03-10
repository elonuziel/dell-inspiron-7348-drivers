# Dell Inspiron 7348 Setup & Drivers

This folder contains essential drivers and information for setting up a Dell Inspiron 7348 laptop on Windows 10 64-bit.

## 📦 Included Drivers
These drivers are version **21.10.1** (Intel official).

1.  **WiFi**: `WiFi_21.10.1_64_Win10.exe`
    *   Intel Wireless adapter driver for Windows 10.
    *   Release Notes: `WiFi_21.10.1_ReleaseNotes.pdf`
2.  **Bluetooth**: `BT_21.10.1_64_Win10.exe`
    *   Intel Bluetooth adapter driver for Windows 10.
    *   Release Notes: `BT_21.10.1_ReleaseNotes.pdf`

---

## 🛠️ Essential Tools & Troubleshooting

### 1. Battery & Performance: ThrottleStop
If your laptop is extremely slow (locked at 800MHz) or the battery is not charging, it is likely due to a Dell power identification issue (e.g., faulty AC adapter or DC jack).

*   **Issue**: The BIOS triggers **BD PROCHOT** when it cannot identify the charger, which throttles the CPU and often prevents battery charging.
*   **Solution**: Use **ThrottleStop** to bypass this.
    *   **Action**: Uncheck the **BD PROCHOT** box in the main ThrottleStop window.
    *   **Result**: This will restore your CPU to its full speed. Note that if the hardware (charger/DC jack) is physically damaged, the battery may still refuse to charge, but the laptop will be usable again.

### 2. Fan Control: NoteBookFanControl (NBFC)
The Dell Inspiron 7348 can sometimes have aggressive or inefficient BIOS fan curves.

*   **Tool**: Download and install **NoteBookFanControl**.
*   **Configuration**:
    1.  Open NBFC.
    2.  Click the "..." button to browse for a configuration.
    3.  Select the **"Dell Inspiron 7348"** profile (it is included in the official NBFC config library).
    4.  Enable the service to take manual or automated control of the fan speed.

---

## 🔗 Useful Links
*   [Intel Driver Support](https://www.intel.com/content/www/us/en/support/detect.html)
*   [ThrottleStop (TechPowerUp)](https://www.techpowerup.com/download/techpowerup-throttlestop/)
*   [NoteBookFanControl (GitHub)](https://github.com/hirschmann/nbfc)
