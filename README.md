# City3D Public Client

City3D is a Windows desktop package for selecting an address or site, reviewing the map location, extracting nearby OSM/GIS context, and producing City3D reports through the hosted City3D license proxy.

## Download

Download the current public trial ZIP from the latest release:

[City3D-public-trial-2026.5.10.zip](https://github.com/SemPy-debug/city3d-public-client/releases/download/v2026.5.10-public-trial/City3D-public-trial-2026.5.10.zip)

Machine-readable release metadata is available in [`latest.json`](latest.json).

## Public Trial License

The public ZIP includes a preinstalled shared demo license. It is intended for evaluation only.

- Trial length: 7 days from the first successful online license check.
- Machine limit: up to 3 distinct machines total for the shared public demo key.
- Same machine: restarting, moving the folder, or downloading again on the same PC reuses the same machine slot.
- Fourth machine or expired/revoked trial: City3D prints `For free licence or licence request contact: amvrazis.s@gmail.com`.
- Internet is required because the license server uses Render server time. Changing the local Windows clock will not extend a license.

For a private evaluation key, renewal, more machines, or production access, contact [amvrazis.s@gmail.com](mailto:amvrazis.s@gmail.com).

## How To Run On Windows

1. Download the ZIP from the release.
2. Extract it to a normal writable folder, for example `C:\City3D`.
3. Open `City3D\City3D.exe`.
4. Keep the terminal window open. City3D starts its local viewer/server and opens the interactive terminal workflow.
5. Type a place or address, review the map selection, then confirm the location.

Windows 10 or Windows 11 is enough. The package contains its Python runtime and required application files. You do not need to install Python, Ollama, Qwen, DeepSeek, Mapillary tooling, or GIS libraries.

## What Is Included

- `City3D.exe` Windows launcher.
- The local City3D web viewer and CLI workflow.
- The GIS/runtime dependencies needed by the package.
- `config/license.env` containing only the public demo license and Render proxy URL.
- Road 360 helper assets used by report generation.

API keys are not included in the ZIP. DeepSeek Pro Max research, Qwen3-VL vision checks, and Mapillary proxy access run through the hosted Render license proxy after the license check passes.

## Updates

When a new version is available, City3D prints an update notice in the terminal. Press `U` when prompted to update.

The updater downloads the release ZIP, verifies the SHA256 checksum from Render, replaces files in the same folder you launched from, preserves your local `config\license.env`, preserves local license status, and reopens `City3D.exe`.

Current version: `2026.5.10`

## Troubleshooting

- License server unreachable: check that the PC has internet access and can reach `https://city3d-license-proxy.onrender.com`.
- Trial is full or expired: contact `amvrazis.s@gmail.com` for a new key.
- Windows SmartScreen warning: choose more information and run anyway if you trust this release source.
- Do not edit `config\license.env` unless you are pasting a replacement key from support.
- Generated reports are written under the package output folders; keep the package in a writable location.

## Security And Privacy

The client package does not contain operator API keys. The license server validates the license and machine fingerprint hash online before hosted AI or panorama proxy calls. License rules can be renewed, revoked, reduced, expanded, or deleted server-side without sending a new EXE.

## Support

Email: [amvrazis.s@gmail.com](mailto:amvrazis.s@gmail.com)
