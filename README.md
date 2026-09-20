# EnergyAI Status

Public transport repository for the EnergyAI tablet dashboard.

## Important

This repository must contain **only encrypted monitoring payloads**.

- `app-status.enc.json` is encrypted with AES-256-GCM before it leaves the private EnergyAI repository.
- FoxCloud, RABOT, OpenAI and GitHub credentials must never be committed here.
- Plaintext `app-status.json` must never be committed here.
- The Android tablet will later fetch the encrypted file and decrypt it locally.

Stable raw endpoint after the first successful publish:

```
https://raw.githubusercontent.com/herby537/EnergyAI-Status/main/app-status.enc.json
```

The encryption key is not stored in this repository.
