# Matudlo ECD Checklist — releases

Downloads for **Matudlo ECD Checklist**, a Windows app that fills in the
Philippine ECD Checklist (Kindergarten) for teachers: it counts the raw
scores, looks up every scaled score, finds the standard score and reads the
interpretation.

**[Download the latest version](../../releases/latest)**

This repository holds installers only — there is no source code here.

## Installing

1. Download `MatudloECD_Setup_vX.Y.Z.exe` from the
   [latest release](../../releases/latest) and run it.
2. Windows SmartScreen will say the publisher is unrecognised, because the
   installer is not code-signed yet. Choose **More info → Run anyway**.
3. Open the app and click **Activate**, then paste the product key from your
   Matudlo Store receipt.

Encoding your class and saving your files is free. Printing and exporting
need a product key.

## Verifying a download

Every release includes `SHA256SUMS.txt`. To check a file yourself, in
PowerShell:

```powershell
Get-FileHash .\MatudloECD_Setup_v1.0.0.exe -Algorithm SHA256
```

Compare the result with the line in `SHA256SUMS.txt`. The app's own updater
does this automatically and refuses to run an installer whose hash does not
match.

## Support

Buy a key and get help at [matudlo.com](https://matudlo.com/).
