# OpenCFG

**OpenCFG is an Android client for SSH, V2Ray/Xray, WireGuard, DNSTT, and SlipStream configurations.**

[![Latest Release](https://img.shields.io/github/v/release/noahclanman/OpenCFG-Client-App-Public?label=Latest%20Release\&include_prereleases)](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/noahclanman/OpenCFG-Client-App-Public/total?label=Downloads)](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases)
[![Android](https://img.shields.io/badge/Android-6.0%2B-3DDC84?logo=android\&logoColor=white)](#requirements)

OpenCFG provides a simple way to import, manage, and connect to network configurations directly from Android.

## Features

### Supported Protocols

* SSH
* V2Ray / Xray
* WireGuard
* DNSTT
* SlipStream

### Configuration

* Import configurations from URI links
* Import configuration files
* QR code configuration import
* Subscription link support
* Payload configuration
* TLS configuration
* Full-device VPN routing
* Connection logs for diagnostics
* Locked and managed configuration support

## Requirements

* Android 6.0 (Marshmallow) or newer
* Package name: `com.shinu.opencfg`

## Installation

1. Go to the [Releases](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases) page.
2. Download the latest APK.
3. If Android blocks the installation, allow your browser or file manager to install unknown apps.
4. Open the APK and follow the installation instructions.

> **Important:** Only download OpenCFG from the official GitHub repository or trusted OpenCFG distribution channels. Avoid modified or unofficial APKs.

## Getting Started

1. Obtain a valid OpenCFG configuration.
2. Open OpenCFG.
3. Tap **Add Profile**.
4. Import your configuration using a URI, file, QR code, or subscription link.
5. Select the imported profile.
6. Tap **Connect**.

Once connected, OpenCFG routes device traffic through the selected configuration according to its supported protocol and settings.

## Profiles

OpenCFG uses profiles to organize your connection configurations.

A profile can contain the information required to establish a connection, including:

* Server information
* Protocol settings
* Authentication details
* Payload settings
* TLS settings
* VPN routing configuration

Profiles can be imported, managed, and connected directly from the application.

## Connection Logs

OpenCFG provides connection logs to help diagnose connection and configuration problems.

Logs can be useful when troubleshooting:

* Connection failures
* Authentication errors
* TLS errors
* Payload problems
* Server connection issues
* Protocol errors

When sharing logs for support, remove passwords, private keys, tokens, UUIDs, and other sensitive information first.

## Support

### OpenCFG Website

For account, configuration, or service-related support:

**[opencfg.xyz](https://opencfg.xyz)**

### GitHub Issues

For application bugs and technical issues:

**[Open an issue](https://github.com/noahclanman/OpenCFG-Client-App-Public/issues)**

When reporting a bug, include:

* OpenCFG version
* Android version
* Device model
* Protocol being used
* Relevant log output
* Steps to reproduce the problem

Do not include private credentials or sensitive configuration data.

## Disclaimer

OpenCFG is a client application and does not provide VPN or proxy services by itself.

A valid configuration or service endpoint is required to establish a connection.

Users are responsible for ensuring that their use of OpenCFG and any connected network services complies with the laws and regulations applicable to them.

## Links

* **Website:** https://opencfg.xyz
* **GitHub:** https://github.com/noahclanman/OpenCFG-Client-App-Public
* **Releases:** https://github.com/noahclanman/OpenCFG-Client-App-Public/releases
* **Issues:** https://github.com/noahclanman/OpenCFG-Client-App-Public/issues

---

**OpenCFG**
Android network configuration client.
