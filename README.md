# SentriSphere appliance releases

Install SentriSphere Intruder Edge on a supported Seeed reComputer RK3576 with
one terminal command. Use the Debian 12/bookworm vendor image with kernel
`6.1.115-vendor-seeed-rk3576`, a non-root account with sudo access, Python 3.11
or newer, and an internet connection.

```sh
curl -fsSL https://github.com/hasantavision/sentrisphere-releases/releases/download/rk3576-2026.10.12/install.sh | sh
```

The installer requests sudo when needed and prints the dashboard URL. Open that
URL on the same network; the default port is `5175`. Choose **Create Master User**
to create your cloud account, then configure your cameras in the dashboard.
Installation leaves account creation and camera setup to you.

The hosted installer passed its first installation and hardware initialization
checks, and the Create Master User registration form rendered in the browser.
Acceptance used fresh application/database volumes on the existing RK3576 board
at port `5176`, reusing its vendor OS and Docker installation. The hardware
profile remains **unqualified** for detector accuracy and sustained camera
capacity.

Repeating the same installer preserved the test installation's secrets, data
and containers. The existing pilot remained unchanged and healthy.

This is an online installer. Native runtime files are downloaded directly from
Rockchip and Seeed; offline installation is unavailable. The model is distributed
under the owner's confirmed Ultralytics Enterprise licence. Upstream notices and
provenance remain in the release assets.

See the [rk3576-2026.10.12 release](https://github.com/hasantavision/sentrisphere-releases/releases/tag/rk3576-2026.10.12)
for download hashes, compatibility records, acceptance limits and
[release notices](https://github.com/hasantavision/sentrisphere-releases/releases/download/rk3576-2026.10.12/RELEASE-NOTICES.md).
The [installation acceptance record](https://github.com/hasantavision/sentrisphere-releases/releases/download/rk3576-2026.10.12/INSTALLATION-ACCEPTANCE.json)
documents the tested scope.
