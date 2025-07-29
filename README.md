# Codec Configuration Tool

A web-based interface for managing codec device configurations and generating JSON device files.

## Overview

This tool provides an intuitive web interface for configuring multiple codec devices and generating a standardized `devices.json` file. It's designed for network administrators and technicians who need to manage codec configurations efficiently.

## Features

- **Dynamic Device Management**: Add and remove codec configurations on the fly
- **Comprehensive Configuration**: Configure all essential codec parameters:
  - Hardware type selection
  - IP address and port settings
  - Authentication credentials
  - Custom device naming
- **Real-time Preview**: Live JSON preview as you configure devices
- **Export Functionality**: Generate and download `devices.json` file
- **Modern Dark UI**: Professional dark theme interface
- **Responsive Design**: Works on desktop and mobile devices

## Supported Hardware Types

- GATEWAY_4
- SCOOP_6
- ENCODER_H264
- DECODER_H264
- SWITCH_IP
- ROUTER_4G
- AUTRE (Other)

## Configuration Fields

Each codec device includes the following configurable parameters:

| Field         | Description               | Example       |
| ------------- | ------------------------- | ------------- |
| Hardware Type | Type of codec device      | GATEWAY_4     |
| IP Address    | Device IP address         | 192.168.1.100 |
| Port          | Control port              | 80            |
| Username      | Authentication username   | admin         |
| Password      | Authentication password   | password123   |
| Custom Name   | User-friendly device name | Main Gateway  |

## Usage

1. Open the HTML file in any modern web browser
2. Click "Add Codec" to create a new device configuration
3. Fill in the device parameters for each codec
4. Review the real-time JSON preview
5. Click "Generate devices.json" to download the configuration file

## Generated JSON Format

The tool generates a JSON file with the following structure:

```json
{
  "codec_01": {
    "hardware_type": "GATEWAY_4",
    "ctrl_ip_address": "10.0.20.220",
    "ctrl_ip_port": "80",
    "ctrl_ip_user": "admin",
    "ctrl_ip_password": "RtS_L@us@nne.Ga",
    "hardware_custom_name": "Gateway"
  },
  "codec_02": {
    "hardware_type": "SCOOP_6",
    "ctrl_ip_address": "192.168.1.70",
    "ctrl_ip_port": "6000",
    "ctrl_ip_user": "admin",
    "ctrl_ip_password": "",
    "hardware_custom_name": "Scoop 6S"
  }
}
```

## Installation

No installation required. Simply:

1. Download the HTML file
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. Start configuring your devices

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Technical Details

- **Frontend**: Pure HTML5, CSS3, and JavaScript (ES6+)
- **Storage**: In-memory storage (no external dependencies)
- **Export**: Client-side JSON file generation
- **Styling**: Modern CSS with dark theme
- **Responsive**: Mobile-friendly design

## Security Notes

- All data is processed client-side
- No data is transmitted to external servers
- Passwords are handled locally and included in the generated JSON
- Consider secure handling of the generated JSON file containing credentials

## Contributing

This is a standalone tool. For modifications:

1. Edit the HTML file directly
2. Test in multiple browsers
3. Ensure JSON output format remains consistent

## License

Open source - feel free to modify and distribute as needed.

## Support

For issues or feature requests, please refer to your system administrator or the development team that provided this tool.
