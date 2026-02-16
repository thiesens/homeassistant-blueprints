# Home Assistant Blueprints

A collection of Home Assistant automation blueprints for enhanced home control.

## Blueprints

### Niko

#### Digital Black Virtual Entities

These blueprints sync virtual entities in Niko Home Control with actual devices via Home Assistant, enabling full control through the Niko Digital Black wall display while keeping state synchronized across all interfaces.

##### Niko Dimmer Sync

Synchronizes a virtual dimmer in Niko Home Control with an actual dimmer (e.g., Philips Hue dimmer).

This blueprint enables control of a dimmer on the Niko Digital Black screen by maintaining sync between:
- **Virtual dimmer**: Niko Home Control virtual dimmer entity
- **Physical dimmer**: Actual dimmer device (e.g., Philips Hue dimmer)

**Features:**
- Two-way or one-directional synchronization
- Syncs brightness and color attributes
- Configurable delay to prevent sync loops

##### Niko Cover Sync

Synchronizes a virtual cover (blinds/shades) in Niko Home Control with an actual cover device (e.g., Somfy, Velux).

This blueprint solves the problem of controlling windows on the Niko Digital Black screen by maintaining sync between:
- **Virtual cover**: Niko Home Control virtual cover entity
- **Actual cover**: Physical window/blind device (e.g., Somfy, Velux)

Control your windows via the Niko app/screen and the actual device will move. Control via Home Assistant or the integrated app and the Niko screen updates.

**Features:**
- Two-way synchronization (bidirectional)
- Syncs position (0-100%) and tilt position
- Configurable delay to prevent sync loops
- Works with any Home Assistant cover device

## Installation

The blueprints are hosted on GitHub and can be imported directly into Home Assistant:

1. In Home Assistant: **Settings → Automations & Scenes → Create Automation → Choose Blueprint**
2. Click **"Browse Blueprints"** and search for the blueprints by name, or
3. Use the **"Browse Blueprint Community Blueprints"** option

Alternatively, import directly using the repository URL.

## Configuration Examples

### Niko Dimmer Sync
- **Virtual Dimmer**: Select your Niko virtual dimmer entity
- **Physical Dimmer**: Select your actual dimmer device
- **Sync Direction**: Choose two-way or directional sync

### Niko Cover Sync
- **Actual Cover Device**: Select your Somfy/Velux or other physical cover
- **Virtual Niko Cover**: Select your Niko virtual cover entity
- **Sync Delay**: Default 1.5 seconds (adjust if needed)

## Usage

For more information on using Home Assistant blueprints, see the [official documentation](https://www.home-assistant.io/docs/automation/using_blueprints/).

## License

These blueprints are provided as-is for personal use.
