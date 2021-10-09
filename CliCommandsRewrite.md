# Updated CLI command reference

| Old command\argument | New Command | Description |
| ---         | ---         | ---         |
| NA          | `meadow port` | Get the device port to be used. |
| `meadow --ListPorts` | `meadow port --list` | List all available local serial ports. |
| `--SerialPort <NameOfSerialPort>` | `meadow port --set <port>` | Set the device port to be used. |
| `meadow --help <arg>` | `meadow <verb> --help` | |
| `meadow --Dfu --OsFile <Meadow.OS.bin>` | | |
| `meadow --ClearCache` | `meadow cache --clear` | Clears the CLI's state cache. |
| `meadow --MonoRunState` | `meadow mono` | Reports if the Mono runtime will run after Meadow is restarted. |
| `meadow --MonoDisable` | `meadow mono --disable` | Disable mono from running. |
| `meadow --MonoEnable` | `meadow mono --enable` | Enable mono so it can run. |
| `meadow --MonoFlash` | `meadow mono --flash` | Flashes Mono runtime to the external flash. |
| `meadow --MonoUpdateRt` | `meadow mono --update-rt` | Download runtime files and flashes Mono runtime to flashDownload runtime files and flashes Mono runtime to flash. |
| `meadow --WriteFile file[,file,...] [targetFileName[,targetFileName,...]]` | `meadow file write <file-path[,...]> [<target-file-name>,...]` | |
| `meadow --DeleteFile file[,file,...]` | `meadow fs delete <file-name>[,...]` | |
| `meadow --ListFiles` | `meadow fs --list` | List all files in Meadow partition. |
| `meadow --ListFilesAndCrcs` | `meadow fs --list --crc` | List all files and CRCs in a Meadow partition. |
| `meadow --RenewFileSys` | `meadow fs --recreate` | Recreate the Meadow File System. |
| `meadow --GetDeviceInfo` | `meadow --info` | |
| `meadow --GetDeviceName` | `meadow --name` | |
| `meadow --EraseFlash` | `meadow flash --erase` | Delete all content in Meadow flash. |
| `meadow --VerifyErasedFlash` | `meadow flash --verify-erased` | |
| `meadow --Esp32ReadMac` | `meadow esp32 --read-mac` | |
| `meadow --Esp32Restart` | `meadow esp32 --restart` | |
| `meadow --Esp32WriteFile --McuDestAddr <address> --File <file-path>` | `meadow esp32 --write --mcu-address <address> --file <file-path>` |  Write an external file to ESP32's internal flash. |
| `meadow --FlashOS` | `meadow os --flash` | DFU flash Meadow OS. |
| `meadow --ResetMeadow` | `meadow os --restart` | Restarts the Meadow.OS. |
| `meadow --SetTraceLevel \| -t --TraceLevel 0, 1, 2, 3` | `meadow os trace --trace-level <0, 1, 2, 3>` | |
| NA | `meadow os trace --trace-level` | |
| `meadow --TraceEnable` | `meadow os trace --enable` | Request Meadow to send internal trace messages. |
| `meadow --TraceDisable` | `meadow os trace --disable` | Prevent Meadow from sending internal trace messages (default). |
| `meadow --Uart1Trace` | `meadow os trace --uart1` | Routes Meadow OS trace information to COM1 (UART1) Tx=D12, RX=D13. |
| `meadow --Uart1Apps` | `meadow os trace --free-uart1` | Frees COM1 for Meadow application use (default). |
| `meadow --StartDebugging --VSDebugPort <port>` | `meadow os debugging start --VSDebugPort <port>` | |
