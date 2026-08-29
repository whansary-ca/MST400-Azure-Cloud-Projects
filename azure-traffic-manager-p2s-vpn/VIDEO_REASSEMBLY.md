# Reassembling the Project Video

The original MST400 Project 2 recording is stored in two parts because of GitHub file-size limits.

From the `azure-traffic-manager-p2s-vpn` folder, combine the parts in order.

## Linux / macOS

```bash
cat MST-400-Project-2.mkv.part01 MST-400-Project-2.mkv.part02 > MST-400-Project-2.mkv
```

## Windows PowerShell

```powershell
Get-Content MST-400-Project-2.mkv.part01, MST-400-Project-2.mkv.part02 -Encoding Byte -ReadCount 0 | Set-Content MST-400-Project-2.mkv -Encoding Byte
```

The resulting `MST-400-Project-2.mkv` is the original project recording.
