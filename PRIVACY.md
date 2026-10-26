# OpenCFG Privacy Policy

Last updated: 26 October 2026

This policy describes how the OpenCFG Android application handles information. Websites, VPN servers, subscription providers, and other external services have their own privacy practices.

## Information Stored on Your Device

OpenCFG stores information needed to manage your connections, including:

- Profiles, server addresses, and protocol settings
- Credentials, certificates, and keys included in your configurations
- Application preferences and routing settings
- Connection diagnostics
- Usage history, including server names, protocols, connection counts, connected time, and estimated traffic totals

Saved profiles use encrypted application storage. Settings and usage statistics are stored in the application’s private storage.

Usage history is retained locally for up to 90 days. OpenCFG’s usage overview does not upload this history as analytics.

Exported files, copied configurations, and shared logs are outside the protection of the app’s internal storage.

## VPN Connections

OpenCFG uses Android’s VPN service to route traffic according to your selected configuration and settings.

To establish a connection, the application communicates with your configured VPN server, proxy, DNS resolver, or transport endpoint. These services receive connection information, such as your connecting IP address and any authentication details required by the configuration.

What a server operator can observe depends on the protocol, routing configuration, and encryption used by the applications generating the traffic. OpenCFG does not control independently operated servers.

## IP Address and Location Lookups

The connection map and IP lookup tools contact external services to obtain public IP and approximate location information.

Current lookup services include:

- `api.ip.sb`
- `ipwho.is`
- Cloudflare’s diagnostic endpoint

These services receive the IP address used to reach them. This may be your direct network IP or your VPN exit IP, depending on the lookup and connection state.

Map locations are estimated from IP addresses. The app does not require GPS location permission for this feature.

## Diagnostics and Network Tools

Latency checks and network utilities send requests to their test destinations.

Depending on the feature, this can disclose:

- The public IP used for the request
- The hostname or URL being tested
- DNS queries
- Normal connection and HTTP request information

The default HTTP latency endpoint is hosted by Cloudflare. CDN detection may query Google Public DNS and contact the hostname being checked.

Automatic latency checks can make repeated requests while enabled. Custom test destinations are controlled by their respective operators.

## Subscriptions and Optional Downloads

When you import or refresh a subscription, OpenCFG contacts the subscription URL you provide. Its operator receives your connection information and any token included in that URL.

Optional downloads, such as remote blocking lists, contact the selected hosting service. Only use configuration sources and download URLs you trust.

## Device-Bound Configurations

Protected configurations may use an application-accessible device identifier to check whether a configuration is authorized for the current device.

If you copy or share an identifier with a configuration provider, that provider receives it. Device identifiers should not be posted publicly.

## Permissions

OpenCFG uses permissions for the following purposes:

- **Network access:** Establish connections, resolve hostnames, retrieve subscriptions, and run diagnostics.
- **Network state:** Detect connectivity and network changes.
- **VPN authorization:** Route device traffic through the selected configuration.
- **Foreground service and notifications:** Maintain an active connection and display connection controls.
- **Camera:** Scan configuration QR codes when requested.
- **File access:** Import and export files selected by you. Older Android versions may request storage permission.

The camera is not required for manual configuration or file import.

## Sharing and Support

Information you choose to export or share is sent to the destination you select.

Support messages and GitHub reports may contain your username, device details, logs, or other information you submit. Public GitHub issues are visible to others.

Remove passwords, private keys, tokens, subscription URLs, UUIDs, and device identifiers before sharing logs or screenshots.

## Retention and Deletion

You can remove saved profiles through the application.

Clearing OpenCFG’s application data in Android settings removes its local settings, saved profiles, and usage history. Uninstalling the app normally removes its private application data.

Files exported to shared storage, messages sent to support, public issue reports, and information retained by external providers are not removed by clearing or uninstalling OpenCFG.

## Security

OpenCFG uses Android application isolation and encrypted storage for saved profiles. No storage or transmission method can guarantee complete security.

Configuration protection controls do not replace secure servers, strong credentials, or careful handling of exported files.

## Third-Party Services

External providers process requests under their own policies. Review the policies of your VPN provider, DNS resolver, subscription provider, lookup services, and any custom endpoints you use.

This policy applies to the Android client. It does not describe all processing performed by services linked from the app or repository.

## Changes to This Policy

Updates will be published in this repository with a revised date.

## Contact

For privacy questions, contact the OpenCFG maintainer privately:

[Telegram: @obakesenshi](https://t.me/obakesenshi)

Do not post sensitive information in public issues.
