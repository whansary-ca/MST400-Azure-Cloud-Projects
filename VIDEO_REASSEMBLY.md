# Reassemble the project video

The original video is stored in two parts because the connected upload service limits single encoded requests.

## Linux/macOS

```bash
cat MST-400-Project-2.mkv.part01 MST-400-Project-2.mkv.part02 > MST-400-Project-2.mkv
sha256sum MST-400-Project-2.mkv
```

Expected SHA-256:

```text
4eb7fb360a329eac84655d658768947e4ff2c79d576b7c832927e4e61a9fa89c
```

## Windows PowerShell

```powershell
$parts = @("MST-400-Project-2.mkv.part01", "MST-400-Project-2.mkv.part02")
$out = [System.IO.File]::Create("MST-400-Project-2.mkv")
foreach ($part in $parts) {
    $bytes = [System.IO.File]::ReadAllBytes($part)
    $out.Write($bytes, 0, $bytes.Length)
}
$out.Close()
Get-FileHash "MST-400-Project-2.mkv" -Algorithm SHA256
```
