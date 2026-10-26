# OpenCFG

**An Android network client for SSH, V2Ray/Xray, OpenVPN, and WireGuard, with SlowDNS and Slipstream transport options.**

[![Latest Release](https://img.shields.io/github/v/release/noahclanman/OpenCFG-Client-App-Public?label=Latest%20Release&include_prereleases)](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/noahclanman/OpenCFG-Client-App-Public/total?label=Downloads)](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases)
[![Android](https://img.shields.io/badge/Android-6.0%2B-3DDC84?logo=android&logoColor=white)](#requirements)

[![Support via PayPal](https://img.shields.io/badge/PayPal-Support-003087?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/09274923910)
[![Telegram](https://img.shields.io/badge/Telegram-Message%20Me-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/obakesenshi)
[![Create VPN Account](https://img.shields.io/badge/Create%20VPN%20Account-OpenCFG-00A8E8?style=for-the-badge&logo=protonvpn&logoColor=white)](https://opencfg.xyz)

Import, organize, and connect to network configurations from your Android device. This repository hosts public releases, documentation, and issue reports.

## Features

### Connections

- SSH
- V2Ray / Xray
- OpenVPN
- WireGuard
- SlowDNS (DNSTT) and Slipstream for supported connection types
- Custom payload, TLS, and proxy options
- Full-device VPN routing

Available options depend on the selected protocol and server configuration.

### OpenVPN

- Import `.ovpn` files
- Direct, payload, SSL/TLS, HTTP proxy, and HTTPS proxy modes
- SlowDNS and Slipstream transport options
- Editable server address and port
- Automatic saving of valid profile changes
- Expandable advanced configuration
- Custom payload editor and generator
- Connection logs and tunnel diagnostics

Additional transports require compatible server settings.

### Configuration Management

- Import supported URI links and configuration files
- QR code import
- Subscription links
- Profile and server management
- Configuration import and export
- Locked configurations with optional expiration and device restrictions
- Per-profile automatic server failover

Import methods and configuration options vary by protocol.

### Diagnostics and Network Tools

- Connection map with network and VPN exit locations when available
- Connection latency and transfer-rate display
- HTTP ping, delay tests, and TCP connection tests
- Public IP lookup
- Host-to-IP lookup
- HTTP response checker
- CDN detection using response headers and DNS information
- Connection logs for troubleshooting

Latency results depend on the test method, destination, and network conditions. IP-based location results may differ from a server’s physical location.

### Usage Overview

- Daily, weekly, and monthly summaries
- Estimated download and upload totals
- Connection counts and connected time
- Daily activity charts
- Usage breakdown by server and protocol
- Up to 90 days of locally stored history

Usage estimates may include tunnel overhead and can differ from your provider’s data totals.

### Appearance

Choose **Light**, **Modern**, or **Classic** during initial setup or from the menu and General settings. The connection map follows the selected theme.

## Requirements

- Android 6.0 (Marshmallow) or newer
- A valid server configuration or service endpoint
- Package name: `com.shinu.opencfg`

## Installation

1. Open the [Releases](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases) page.
2. Download the latest APK.
3. If prompted, allow your browser or file manager to install unknown apps.
4. Open the APK and follow the installation instructions.

> Download OpenCFG only from this repository or trusted OpenCFG distribution channels. Avoid modified or unofficial APKs.

## Getting Started

1. Obtain a valid configuration from your server administrator or service provider.
2. Open OpenCFG and add or import a profile.
3. Use a supported URI, configuration file, QR code, or subscription link. For OpenVPN, import your `.ovpn` file.
4. Review the server and authentication settings.
5. Select the profile and tap **Connect**.
6. Approve Android’s VPN permission request when prompted.

Traffic routing follows the selected protocol and application settings.

## Profiles

Profiles organize the servers and settings used for your connections, including:

- Server address and port
- Protocol and transport options
- Authentication details
- Payload and TLS settings
- Routing options

Protected configurations may restrict editing, sharing, or use according to the settings chosen by their creator.

## Connection Logs

Use the logs to investigate connection failures, authentication errors, TLS negotiation, payload responses, and server issues.

Before sharing logs, remove passwords, private keys, tokens, UUIDs, and other sensitive information.

## Support

### Accounts and Services

For account, configuration, or service questions, visit [opencfg.xyz](https://opencfg.xyz).

### Application Issues

Report bugs through [GitHub Issues](https://github.com/noahclanman/OpenCFG-Client-App-Public/issues).

Include:

- OpenCFG version
- Android version and device model
- Protocol and connection mode
- Steps to reproduce the issue
- Relevant logs with sensitive information removed

## License

OpenCFG is proprietary software. This public repository provides application releases and documentation; it does not publish the application’s source code.

Third-party components remain subject to their respective licenses.

## Disclaimer

OpenCFG is a client application. A valid configuration and reachable server are required to establish a connection.

Available features depend on server support and network conditions. Users are responsible for complying with applicable laws and their service provider’s terms.

## Links

- [Website](https://opencfg.xyz)
- [GitHub Repository](https://github.com/noahclanman/OpenCFG-Client-App-Public)
- [Releases](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases)
- [Issue Tracker](https://github.com/noahclanman/OpenCFG-Client-App-Public/issues)
- [Telegram Channel](https://t.me/xray_ehi_hub)
- [Contact on Telegram](https://t.me/obakesenshi)
- [Free V2ray Servers]([https://xm.opencfg.xyz/xvpn/shinu](https://github.com/noahclanman/free-xray-gcp))
- [AIO and Multiplexer Server](https://shinu.opencfg.xyz/xvpn/obake)
