# Ahoy — downloads

Ahoy is a macOS menu-bar app that records and transcribes your calls
(Zoom, Teams, Meet in a browser, …) locally on your Mac.

**Requirements:** macOS 15+ on Apple Silicon.

## Install

1. Download the newest `Ahoy-<version>.dmg` from
   [the Downloads release](https://github.com/razvanbalsan/ahoy-releases/releases/tag/downloads).
2. Open it and drag **Ahoy.app** to **Applications**.
3. **First launch only:** double-click **Ahoy.app** in Applications. macOS
   will say it "could not be opened" — click **Done**. Then open **System
   Settings** → **Privacy & Security**, scroll down to the notice that Ahoy
   was blocked to protect your Mac, click **Open Anyway**, and
   authenticate/confirm when prompted, then click **Open**. Ahoy is signed
   with a personal certificate rather than an Apple Developer ID, so macOS
   asks once. (On macOS versions older than Sequoia you may instead get a
   working **Open** button via right-click → **Open**.)

On first use Ahoy will ask for Microphone and System Audio Recording
permissions — both are needed to transcribe calls.

## Updates

Ahoy checks for updates automatically (Sparkle) and can be updated any time
from the menu bar: **Check for Updates…**
