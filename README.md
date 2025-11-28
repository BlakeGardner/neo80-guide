# neo80 Tri-Mode Keyboard Resources

This site and repository provide a community‑organized collection of helpful information for using the neo80 Tri‑Mode Keyboard by Qwertykeys. While this guide aims to simplify setup and troubleshooting, **always refer to the official Qwertykeys documentation and contact their support team for any issues or assistance.**

## Repository

View the source for this guide or contribute on GitHub:
🔗 **[https://github.com/BlakeGardner/neo80-guide](https://github.com/BlakeGardner/neo80-guide)**

## Connection Instructions

⚡ **Quick Reference:**

* **Fn + Tab** = Cycle connection modes (Esc = wired, 1/2/3 = BT, 4 = 2.4G).
* **Fn + Q/W/E** = Bluetooth slots (pair/switch/reset).
* **Fn + R** = Pair with 2.4G dongle.

### 🔌 Wired Mode

1. Connect the keyboard with the USB-C cable.
2. Press **Fn**, then tap **Tab** until the **LED under Esc** flashes.
3. **LED Behavior:**

   * The LED under Esc flashes 3 times to indicate wired mode.
   * When charging, the Esc LED stays on.
   * The Esc LED turns off when the battery is full.
   * The Esc LED flashes when the battery level is below 5%.

### 📶 Bluetooth Mode

* **Select BT mode:** Press **Fn + Tab** until the **LED under 1 / 2 / 3** flashes 3 times.
* **Pairing a device:**

  1. Hold **Fn + Q / W / E** for **5–10 seconds** until the LED under 1 / 2 / 3 flashes rapidly.
  2. Find the keyboard in your device’s Bluetooth settings and connect.
  3. The LED turns off once pairing is complete.
* **Switching between paired devices:** Tap **Fn + Q / W / E** (short press) to jump to that slot.

  * If connected, the LED flashes 3 times to indicate the paired device.
  * If not connected, the LED flashes slowly while searching for the device.
  * If no device is paired, all LEDs stay off.
* **Forget/disconnect a device:** Hold **Fn + Q / W / E** for **5–10 seconds** until the LED resets.

### 📡 2.4GHz Wireless Mode

1. Remove the dongle (if plugged in).
2. Press **Fn + Tab** until the **LED under 4** flashes 3 times.
3. Hold **Fn + R** until the LED under 4 flashes rapidly.
4. Plug in the dongle (keep the keyboard within ~20 cm / 8 in).
5. Press any key to test the connection.
6. **LED Behavior:**

   * The LED under 4 flashes briefly during pairing.
   * The keyboard and dongle connect automatically if previously paired.

## Remapping and Customization

1. Download the neo80 definition file from this repository: [neo80_wireless.json](./neo80_wireless.json).
2. Visit the [Via website](https://www.usevia.app/).
3. Click on the Settings icon (gear).
4. Enable "Show Design Tab" if not already enabled.
5. Click on the Design tab.
6. Click "Load Draft Definition" and select the downloaded configuration file.
7. Your browser will ask permission to access the keyboard; allow it.
8. You can now remap keys, create layers, and customize lighting as desired.

## Resetting to Default Keymap

If you ever need to restore your neo80 keyboard back to its **factory default layout**, you can do so easily using VIA.

### 🔄 How to Reset Your Keymap

1. Download the default layout file from this repository: [neo80.default.layout.json](./neo80.default.layout.json).
2. Open the [VIA website](https://www.usevia.app/).
3. Go to **Settings** (gear icon).
4. Make sure **"Show Design Tab"** is enabled.
5. Open the **Design** tab.
6. Click **"Load Draft Definition"** and select the default layout file you downloaded.
7. Switch to the **Configure** tab.
8. Scroll to the **Save + Load** section.
9. Use **"Load Saved Layout"** to restore the factory keymap.

## Reset the Keyboard to Factory Settings

You can restore the keyboard to its factory defaults by clearing the EEPROM. To do this, hold `Fn + Delete` for five seconds. This triggers the built‑in QMK keycode `QK_CLEAR_EEPROM`, which wipes all custom mappings — including Bluetooth pairings — and returns the keyboard to its original factory configuration.

## Upgrading Firmware

1. Download and install **QMK Toolbox**.
2. Download the latest firmware **.bin** file from the official website.
3. Run **QMK Toolbox as Administrator** (right‑click → *Run as administrator*).
4. Click **Open** and select the downloaded `.bin` file.
5. Put the keyboard into **DFU Mode** using the steps below:

   1. Disconnect the keyboard.
   2. Hold **Fn + Esc**.
   3. While holding the keys, plug the keyboard back in.
   4. Release the keys once QMK Toolbox detects a **DFU device**.
6. Click **Flash** to begin installing the firmware.

## Putting the keyboard in DFU mode

1. Open the [VIA configurator](https://www.usevia.app/).
2. Go to the **Configure** tab.
3. Choose a key you don’t normally use (for example, a key on Layer 1 or a function layer).
4. Change its function to **`RESET`** (found under *Special → Bootloader / Reset*).
5. Press that key on your keyboard.

Once pressed, the keyboard will enter **DFU mode**.

### 🖥️ What You’ll See in QMK Toolbox

```
DFU device connected
```

Your keyboard is now in bootloader mode and ready to flash new firmware.

## Useful Resources

* [Official Product Page](https://www.qwertykeys.com/products/neo80)
* [Build Guide](https://qwertykeys.notion.site/Neo80-Build-Guide-a89eb0eca0a0490bbb1fe27a2ef51fb4)
* [Firmware Updates](https://www.qwertykeys.com/pages/fw)
* [Pairing Instructions](https://qwertykeys.notion.site/Pairing-instructions-e45641e8dbfd4b96980d2bc0930fdfa1?p=2003d09009428196b0ffc7f1384cc80b&pm=c)
