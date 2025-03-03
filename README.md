# Overview

Converts 2FAS authenticator backup files to QR codes that can be imported into any other authenticator app.

See: <https://2fas.com/>

This file is modified from https://github.com/mauriciosantos/2fas-to-qr to add uv support.

## Usage

Using the app go to Settings -> Backup -> Export -> Disable Set Password Option -> Export to File

Move the file to a system with uv and execute script:

```bash
./twofas_to_qr.py '<2FAS Input File>' '<Output Directory>'
```

Then scan the generated codes using your authenticator app of preference. Remember to delete the 2FAS backup file as well as generated QR codes afterwards! They contain the plaintext secrets that anyone can see.
