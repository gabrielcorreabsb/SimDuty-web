# SimuDuty - Install Notes

## App
- Run `SimuDuty.exe` from the release package.
- Logs/Saves/Config will be created in:
  - `%LOCALAPPDATA%\SimuDuty\Logs`
  - `%LOCALAPPDATA%\SimuDuty\Saves`
  - `%LOCALAPPDATA%\SimuDuty\Config`
- Key files you may see:
  - `Config/gui_setup.json`
  - `Saves/eld_save_<PLATE>_<TRUCK>.json` (+ `.bak`/`.tmp`)
  - `Saves/eld_audit_<PLATE>_<TRUCK>.jsonl`
  - `Saves/user_save_<DRIVER>_<POLICY>.json`

## Plugins (ATS / ETS)
- The DLLs located in the **plugins** folder must be installed in the game plugins directory:
  - ATS (64-bit): `...\American Truck Simulator\bin\win_x64\plugins`
  - ATS (32-bit): `...\American Truck Simulator\bin\win_x86\plugins`
  - ETS2 (64-bit): `...\Euro Truck Simulator 2\bin\win_x64\plugins`
  - ETS2 (32-bit): `...\Euro Truck Simulator 2\bin\win_x86\plugins`

## Troubleshooting
- If SimuDuty does not connect, verify the plugin DLLs are in the correct game plugins folder.
- Open the Debug tab and confirm the DLL status is OK and `GET_GAME_TIME_INFO` returns a source.
