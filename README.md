# Home Assistant Blueprints

A collection of Home Assistant automation blueprints for enhanced home control.

## Blueprints

### Niko Dimmer Sync

Synchronizes a virtual dimmer in Niko Home Control with an actual dimmer (e.g., Philips Hue dimmer).

This blueprint enables control of a Hue dimmer on the Niko digital black screen by maintaining sync between:
- **Virtual dimmer**: Niko Home Control virtual dimmer entity
- **Physical dimmer**: Actual dimmer device (e.g., Philips Hue dimmer)

#### Requirements

- Home Assistant instance with Niko Home Control integration
- Physical dimmer device (e.g., Philips Hue dimmer)
- Automation support enabled

#### Installation

1. Copy the blueprint file to your Home Assistant blueprints directory:
   ```
   blueprints/automation/niko_dimmer_sync.yaml
   ```

2. Create automations from the blueprint via Settings → Automations & Scenes → Create Automation → Choose Blueprint

#### Configuration

Select the following when creating an automation from this blueprint:
- **Virtual Dimmer**: The Niko Home Control virtual dimmer entity
- **Physical Dimmer**: The actual dimmer device to sync with
- **Synchronization Direction**: Two-way, virtual to physical, or physical to virtual

## Usage

For more information on using Home Assistant blueprints, see the [official documentation](https://www.home-assistant.io/docs/automation/using_blueprints/).

## License

These blueprints are provided as-is for personal use.
