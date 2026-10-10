# Ahoy — downloads

Ahoy is a macOS menu-bar app that records and transcribes your calls
(Zoom, Teams, Meet in a browser, …). Transcription runs on your Mac or
with a cloud service you choose: Gemini, Soniox, AssemblyAI, ElevenLabs
or OpenAI.

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

## What's new in 2.0.1

- **ElevenLabs fixes:**
  - Ahoy now makes sure ElevenLabs' copy of the transcript is really
    deleted.
  - **Test Connection** succeeds with a working key.
  - A key used with the wrong region now says to check the key and its
    region.

## What's new in 2.0.0

- **Four more transcription services: Soniox, AssemblyAI, ElevenLabs and
  OpenAI.** Each one transcribes the recording after the call, with
  speakers separated and your microphone labelled as you, and gives live
  captions during the call. Both follow your existing **Transcribe
  automatically when a call ends** and **Live captions during calls**
  settings. Pick one under **Settings → Transcription**, or from a call's
  **Transcribe** menu.
- **Settings → API Keys** (renamed from API Key): add a key for each
  service, with a link to the page where you create it, a **Test
  Connection** button and a **Region** picker (Global or EU).
- **You pay the service directly.** Approximate prices per audio hour:

  | Service    | After the call | Live captions |
  |------------|---------------:|--------------:|
  | Soniox     | $0.10          | $0.12         |
  | AssemblyAI | $0.15          | $0.45         |
  | ElevenLabs | $0.22          | $0.39         |
  | OpenAI     | $0.36          | $1.02         |

- **Privacy:**
  - Ahoy deletes the service's copy of the audio and transcript as soon as
    it has the result. OpenAI keeps no copy of after-call audio.
  - AssemblyAI uses its EU region by default, at the same price.
  - EU processing on Soniox needs an EU project and that project's own key
    (ask Soniox support).
  - EU on ElevenLabs is an Enterprise feature, and on OpenAI it needs
    OpenAI's approval.
  - ElevenLabs may use your audio for training unless you turn that off in
    your ElevenLabs account.
- **Gemini:** Settings and the setup wizard now link to Google's guide for
  creating a Gemini API key.

## Updates

Ahoy checks for updates automatically (Sparkle) and can be updated any time
from the menu bar: **Check for Updates…**
