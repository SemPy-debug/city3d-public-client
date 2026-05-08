# Troubleshooting

## The license check fails

City3D requires internet access to `https://city3d-license-proxy.onrender.com`. The server uses online UTC time, so local Windows clock changes do not renew or extend trials.

## The public trial says the machine limit is reached

The public demo key allows 3 distinct machine(s). Contact `amvrazis.s@gmail.com` for a private key.

## I received a private activation key

Run:

```powershell
City3D.exe --activate
```

Paste the key when prompted. City3D writes it to `config\license.env` and verifies it online.

## Updating

When City3D says an update is available, press `U`. The updater works in the same directory and preserves your license file.
