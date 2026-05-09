# City3D Windows Trial

City3D turns an address or development site into a structured property intelligence workspace. Start with a location, review it on the map, and produce a professional site package with building context, parcel context, road evidence, planning research, visual observations, and an exportable HTML report.

It is designed for real estate, architecture, planning, surveying, development, investment screening, and early feasibility work: one portable Windows folder, no Python setup, no separate local AI stack, and no GIS installation.

## Download

Download the current Windows trial ZIP from the latest release:

[City3D-public-trial-2026.5.12.zip](https://github.com/SemPy-debug/city3d-public-client/releases/download/v2026.5.12-public-trial/City3D-public-trial-2026.5.12.zip)

Machine-readable release metadata is available in [`latest.json`](latest.json).

## What You Can Do

- Search a city, street, landmark, parcel area, or exact address.
- Review the selected point and site context in the City3D map workflow.
- Extract buildings, parcels, roads, addresses, and local geometry into reusable project files.
- Generate a full due-diligence style HTML report for a selected site.
- Inspect surrounding road and building context with visual evidence where available.
- Use the completed export as a project record, client discussion pack, or feasibility starting point.
- Create separate follow-up reports from the completed project data, such as summaries, memos, tables, or document drafts.

## Trial License

The public ZIP includes a preinstalled shared trial license. It is intended for evaluation only.

- Trial length: 7 days from the first successful online license check.
- Machine limit: up to 3 distinct machines total for the shared public trial key.
- Same machine: restarting, moving the folder, or downloading again on the same PC reuses the same machine slot.
- Fourth machine or expired/revoked trial: City3D prints `For free licence or licence request contact: amvrazis.s@gmail.com`.
- Internet is required because the license is checked against City3D server time. Changing the local Windows clock will not extend a license.

For a private evaluation key, renewal, more machines, or production access, contact [amvrazis.s@gmail.com](mailto:amvrazis.s@gmail.com).

## How To Run On Windows

1. Download the ZIP from the release.
2. Extract it to a normal writable folder, for example `C:\City3D`.
3. Open `City3D\City3D.exe`.
4. Keep the terminal window open. City3D starts its local project workspace and interactive workflow.
5. Type a place or address, review the map selection, then confirm the location.

Windows 10 or Windows 11 is enough. The package contains its runtime and required application files. You do not need to install Python, a local AI server, GIS libraries, or developer tools.

## What Is Included

- `City3D.exe` Windows launcher.
- The local City3D web viewer and CLI workflow.
- The runtime dependencies needed by the package.
- `config/license.env` containing only the public trial license and City3D service URL.
- Report, map, and visual-review assets used by project generation.

Private operator credentials are not included in the ZIP. Hosted City3D services handle licensed online capabilities after the license check passes.

## Where Reports Are Saved

City3D writes exports beside the executable, inside:

```text
City3D\building_outputs\<project-folder>\
```

Each project folder can include the HTML report, GeoJSON files, research JSON, visual-audit JSON, road imagery metadata, and usage summary.

## Updates

When a new version is available, City3D prints an update notice in the terminal. Press `U` when prompted to update.

The updater downloads the release ZIP, verifies the SHA256 checksum, replaces files in the same folder you launched from, preserves your local `config\license.env`, preserves local license status, and reopens `City3D.exe`.

Current version: `2026.5.12`

## Troubleshooting

- License service unreachable: check that the PC has internet access.
- Trial is full or expired: contact `amvrazis.s@gmail.com` for a new key.
- Windows SmartScreen warning: choose more information and run anyway if you trust this release source.
- Do not edit `config\license.env` unless you are pasting a replacement key from support.
- Generated reports are written under the package output folder; keep the package in a writable location.

## Security And Privacy

The client package does not contain private operator credentials. City3D validates the license and a machine fingerprint hash online before hosted capabilities are used. License rules can be renewed, revoked, reduced, expanded, or deleted server-side without sending a new EXE.

## Support

Email: [amvrazis.s@gmail.com](mailto:amvrazis.s@gmail.com)
