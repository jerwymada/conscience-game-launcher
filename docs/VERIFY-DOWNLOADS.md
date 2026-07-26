# Verify Downloads

The SHA-256 checksum confirms that a downloaded file is byte-for-byte identical
to the published artifact. It does not replace code signing, but it detects
corruption or modification.

## PowerShell

Open PowerShell in the download directory:

```powershell
Get-FileHash .\ConscienceGameLauncher-Setup-v1.2.1.exe -Algorithm SHA256
Get-FileHash .\ConscienceGameLauncher-v1.2.1-portable-win-x64.zip -Algorithm SHA256
```

Expected values:

```text
591CAD45D4EB05B9CDCC229D7C17D042554AEBB162521FEDDE70CBC06B528C7D
5D0BEA640ED0758FDFCFB6E1AB13E5A7C59B9675B4E7ED0140C2B8F2A3743048
```

The first value is the Setup; the second is the Portable ZIP.

## Command Prompt

```bat
certutil -hashfile ConscienceGameLauncher-Setup-v1.2.1.exe SHA256
certutil -hashfile ConscienceGameLauncher-v1.2.1-portable-win-x64.zip SHA256
```

## Vérification en français

Compare l'empreinte affichée avec la valeur correspondante dans
[`downloads/SHA256SUMS.txt`](../downloads/SHA256SUMS.txt). Une seule différence
signifie que le fichier ne doit pas être exécuté. Supprime-le et télécharge-le
de nouveau depuis ce dépôt.
