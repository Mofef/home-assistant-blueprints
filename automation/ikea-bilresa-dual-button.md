# IKEA BILRESA Dual Button Remote Automation

## Current Version 3.0.0

## Features

Simple automation blueprint for IKEA BILRESA dual-button remote.

### Supported Actions for Each Button

* Single Press
* Double Press
* Long Press (on press and release)
* While Holding (with configurable interval)

### Configuration Options

* Configurable interval in milliseconds for "while holding" actions.
* Safety limit on maximum iterations for "while holding" actions to prevent infinite loops.

## Requirements

* Requires Home Assistant 2026.8.0 or newer.

### 3.0.0

- Replaced state triggers with event.received triggers for single press, double press, long press, and long release.
- Filtered button event entities by IKEA of Sweden / BILRESA dual button device metadata.
- Changed holding intervals from seconds to milliseconds with new input names.
- Raised the minimum Home Assistant version to 2026.8.0.

[See the 3.0.0 upgrade guide](https://community.home-assistant.io/t/ikea-bilresa-dual-button-remote/965815/48?u=skaronator) for migration instructions and interval conversion examples.

### 2.0.1

- Removed Matter integration filter for button event selector. This will allow users to use the Ikea BILRESA remote over 3rd party Matter integration.

### 2.0.0

- Added support for selecting multiple entities for each button. Allowing to have multiple remotes triggering the same actions.
- See the [2.0.0 migration guide](https://community.home-assistant.io/t/ikea-bilresa-dual-button-remote/965815/28?u=skaronator) for upgrading existing automations.

### 1.2.2

- Improved descriptions and documentation.

### 1.2.1

- Improved descriptions for blueprint inputs.

### 1.2.0

- Added max iterations setting for "while holding" actions to prevent infinite loops.

### 1.1.0

- Added "while holding" actions for both buttons with configurable interval.

### 1.0.0

- Initial release with support for all button actions.

## Support and Feedback

* GitHub: [Skaronator/home-assistant-blueprints](https://github.com/Skaronator/home-assistant-blueprints)
* Blueprint Exchange: [IKEA BILRESA Dual Button](https://community.home-assistant.io/t/ikea-bilresa-dual-button-remote/965815)

Thank you for using this blueprint! Your feedback and contributions are welcome.
