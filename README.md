# NVCP Toggle GUI

NVCP Toggle GUI is a lightweight Windows utility for switching NVIDIA Control Panel image settings between two states: a normal monitor profile and a custom gameplay profile.

It was created as a more polished, easier-to-use version of the original NVCP Toggle project on GitHub. The goal is simple: make display adjustments fast, reversible, and convenient without forcing you to open the NVIDIA Control Panel every time or permanently change your monitor’s usual configuration.

## Why this exists

I mainly use this tool for games like **Escape from Tarkov**, where visibility matters a lot. In games like that, a small change in vibrance, gamma, brightness, contrast, or hue can make a real difference. The problem is that changing those values manually in the NVIDIA Control Panel every time is slow and inconvenient.

NVCP Toggle GUI solves that by letting you:

* create a custom visibility profile,
* test it immediately,
* toggle back to your normal configuration when you are done,
* and restore the exact state you captured before applying changes.

That makes it useful not only for Escape from Tarkov, but for any game or use case where you want temporary display tuning without permanently affecting your monitor setup.

## Features

* Modern **Windows 11-style dark UI**
* Minimalist interface with clean spacing and simple controls
* Custom sliders for image tuning
* Live preview / test mode
* Toggle between a gameplay profile and a restored baseline
* Exact restoration of the previous display state
* Support for the following NVIDIA settings:

  * Digital Vibrance
  * Hue
  * Brightness
  * Contrast
  * Gamma
* Quick toggle mode for fast switching
* Saved configuration in a local JSON file
* Captured restore state stored separately for reliability

## How it works

The application works with two display states:

### 1. Gameplay profile

This is the configuration you want while playing. You can adjust the sliders and apply the values immediately to test how the image looks in real time.

### 2. Restore profile

This is the state used to return the display to normal. By default, the app can capture your current settings before applying the gameplay profile, so the restore step brings you back to the exact values that were active before the toggle.

This is important because some tools use fixed fallback values. NVCP Toggle GUI is designed to avoid that problem by restoring the real captured state whenever possible.

## Installation

1. Download the latest release for Windows x64.
2. Extract the ZIP file to a normal folder.
3. Run `NVCP Toggle GUI.exe`.
4. Adjust your settings and save your preferred profile.

For quick switching without opening the interface, use `NVCP Toggle Quick.exe`.

## Basic usage

### First time setup

1. Open the GUI version.
2. Choose the profile you want to use.
3. Adjust the sliders until the image looks right.
4. Test the result.
5. Save the configuration.

### Normal use

* Use the GUI when you want to fine-tune the settings.
* Use the quick toggle when you only want to switch states immediately.

### Restore behavior

For the safest workflow, keep automatic restore capture enabled. That way, the app saves your current monitor state before applying changes and restores it later exactly as it was.

## Settings

The app supports adjustments for:

* Digital Vibrance
* Hue
* Brightness
* Contrast
* Gamma

All values are stored locally in the application settings file.

## Notes

* This tool is intended for temporary visual tuning.
* It does not replace NVIDIA Control Panel.
* It is meant to make frequent switching easier.
* Because it works with display settings, results may vary depending on your monitor, GPU, driver version, and Windows configuration.

## Credits

This project is based on the original public **NVCP Toggle** project on GitHub. https://github.com/mcgrizzz/NVCP_Toggle
This fork expands it with a modern UI, a more practical workflow, and better restore behavior for users who want a cleaner day-to-day experience.

## License

This project keeps the original licensing terms from the upstream project. Please check the repository license before redistributing or modifying the code.
