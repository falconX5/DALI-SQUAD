# DALI SQUAD Client

Member-only package. It intentionally excludes `server.py`, `access_admin.py`, `access.json`, and admin identity files.

## Setup
Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```
Windows PowerShell:
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Create your identity
```bash
python client.py --show-identity --name HUNT3R
```
Send only the public key and fingerprint to the admin. Never send your identity file.

## Connect
```bash
python client.py --server ws://NGROK_HOST:PORT --room dark-room --secret "ROOM_SECRET" --name HUNT3R
```
