# OpenCFG FAQ

## What is OpenCFG?

OpenCFG is an Android client for importing, managing, and connecting to network configurations. A valid configuration and reachable server are required.

## Where can I download the official APK?

Download it from the [OpenCFG releases page](https://github.com/noahclanman/OpenCFG-Client-App-Public/releases) or trusted OpenCFG distribution channels.

Avoid modified APKs from unknown sources.

## What Android version is required?

Android 6.0 or newer.

## Does OpenCFG provide a VPN server automatically?

No. You need a compatible server or configuration from your own server administrator or service provider.

## How do I import a configuration?

Use the import option for your configuration type. Supported methods include files, URI links, QR codes, and subscription links.

Not every format is supported by every protocol.

## How do I import an OpenVPN profile?

Open the OpenVPN editor and select **Import .ovpn**.

The app loads the configuration and fills the primary server address and port. Enter a username and password if your server requires them, then review the connection mode.

## Can I change the OpenVPN address without editing the configuration text?

Yes. Edit the **Address** and port fields.

OpenCFG updates the primary remote entry while preserving certificate content and fallback server entries.

## Why is the OpenVPN configuration hidden?

Advanced configuration is collapsed to keep the editor easier to use. Select **Show** to view or edit it.

## Does OpenVPN save changes automatically?

Valid changes save automatically after a short pause. Check the save status before leaving the editor.

Incomplete or invalid settings may need correction before they can be saved. Protected configurations can restrict editing.

## Will every OpenVPN server work with payload, TLS, proxy, SlowDNS, or Slipstream?

No. These modes require compatible server and transport settings.

Importing an `.ovpn` file does not add those capabilities to its server.

## Why does Android ask for VPN permission?

Android requires your approval before an application can create a VPN connection and route device traffic.

## Why does the app say connected, but websites do not load?

A connected tunnel does not always mean the server can reach the internet.

Check:

- Server routing and internet access
- DNS settings
- Account validity
- Payload, proxy, and TLS settings
- Server support for the selected transport
- Connection logs

For slow DNS transports, allow additional time for requests to complete.

## Why is OpenCFG’s latency different from another app?

Apps can measure different things.

ICMP ping measures packet round-trip time. TCP tests measure connection establishment. HTTP and HTTPS tests measure a request to a test endpoint, potentially including connection and TLS setup.

Results also depend on the destination, server routing, connection reuse, and current network conditions. Compare apps using the same test method and endpoint where possible.

## Why can the first latency result take longer?

The tunnel, DNS resolution, and test connection may still be initializing. Later requests can benefit from cached information and established connections.

OpenCFG performs readiness checks and connection warm-up to reduce this effect.

## Why does latency show “Unavailable” or “Timeout”?

The test endpoint may be unreachable, blocked, or too slow to respond within the test limit.

This does not always mean the tunnel is disconnected. Try opening a website and checking the logs.

## Why is the map location wrong or missing?

The map uses public IP location databases. Their information may be incomplete, outdated, or associated with a provider’s registered location.

A VPN exit location can also differ from the physical server location because of upstream routing or relays.

## Are usage totals the same as my mobile provider’s totals?

Not necessarily.

OpenCFG estimates app activity while connected. Tunnel overhead, retransmissions, loopback traffic, and provider accounting can produce different totals.

Use your provider’s records for billing.

## How long is usage history kept?

Up to 90 days, stored locally on your device.

## How do I change the theme?

Open the theme option in the menu or General settings and choose **Light**, **Modern**, or **Classic**.

The connection map follows your selection.

## Why can’t I edit or export a configuration?

Its creator may have enabled protection restrictions. Protected configurations can also be limited by expiration or device binding.

Contact the configuration provider if access needs to be changed.

## Does CDN Finder always identify the CDN?

No. It checks available DNS and response-header evidence. Some services hide their infrastructure or provide no reliable indicators.

An unknown result does not prove that a domain has no CDN.

## Can I update without losing my profiles?

Installing an official update over the existing app normally preserves its data.

Uninstalling OpenCFG or clearing its application data removes locally stored profiles and settings. Export configurations you are permitted to back up before doing either.

## How do I report a problem?

Open an issue in the [issue tracker](https://github.com/noahclanman/OpenCFG-Client-App-Public/issues).

Include:

- OpenCFG version
- Android version and device model
- Protocol and connection mode
- Steps to reproduce the issue
- Relevant logs with sensitive information removed

Never post credentials, private keys, subscription tokens, or device identifiers.

## Where can I read the privacy policy?

See [PRIVACY.md](PRIVACY.md).
