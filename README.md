# BDO Loot Tracker

Tracks your Black Desert Online grind sessions: loot, silver, kills and Agris usage, with a live loot window.

## Install

1. **Download** the latest installer from the [Releases](https://github.com/Yoind/BDO-loot-tracker/releases) page and run it.
2. **Install Python 3.10.6** from [python.org](https://www.python.org/downloads/release/python-3106/).
   Tick **Add Python to PATH** on the first screen of the installer.
3. **Install scapy.** Open Command Prompt and run:
   ```
   pip install scapy
   ```
4. Pick how the app reads game packets, then start the app.

## Packet capture

The app reads the game's network packets to see your loot. Pick one method in **Settings - Tracking - Packet Capture**.

### Without Npcap (recommended)

Nothing else to install.

1. Set **Method** to **Windows raw sockets (no Npcap)**.
2. Run the app **as administrator**. If it isn't, it will ask to restart as admin and will keep starting that way.
3. If you use a VPN or several network adapters, pick yours under **Adapter**. Automatic works for most people.

### With Npcap

1. Install [Npcap](https://npcap.com/#download).
2. Set **Method** to **Npcap**.

## Tips

- Setup the keybinds.
- Start tracking before your first kill.
- Changes to the capture method apply the next time tracking starts.
- If loot isn't being counted, check that Python is on your PATH: `python --version` should print `3.10.6`.
