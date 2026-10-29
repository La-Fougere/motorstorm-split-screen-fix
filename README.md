# motorstorm-split-screen-fix

An RPCS3 profile for fixing split-screen rendering issues in **MotorStorm: Pacific Rift**, without disabling shadows or visual effects.

**Likely cause:** RPCS3's automatic preset can force `MSAA: Disabled` despite your global settings. A game-specific custom profile prevents that override.

**For game ID BCES00129, update 1.03.**

## Quick start

1. Click **Code → Download ZIP** at the top of this repository, then extract the archive.
2. **Close RPCS3.** Copy [`config_BCES00129.yml`](config_BCES00129.yml) to the following location inside your RPCS3 installation:

   ```text
   config/custom_configs/config_BCES00129.yml
   ```

   Create `custom_configs` if needed. **Back up any existing file before replacing it.**

3. Open RPCS3 and **double-click the game as usual**. The settings are applied automatically.

**No `.cmd` file, terminal, or script is required.** Do not use a boot option that ignores the game's custom configuration.

## Notes

- **Resolution:** the profile renders at **1440p**. To reduce the load, change `Resolution Scale: 200` to `Resolution Scale: 100` (720p).
- **Four players:** in RPCS3's controller settings, assign a different controller to each of ports 1–4. This file does not replace your controller profiles.
- **Other editions:** this file is specific to **BCES00129**. It is not applied automatically to other game IDs.
- **Undo:** close RPCS3 and restore your previous profile. If you had no custom profile before, simply remove the file added here.

This repository contains only the guide and settings: no game, firmware, or modified RPCS3 binaries.

### References

- [AA/AF settings and split-screen rendering issues](https://github.com/RPCS3/rpcs3/issues/14758)
- [Custom configuration precedence in RPCS3](https://github.com/RPCS3/rpcs3/blob/6c44fff7549e941389a4ce072a95c5ff9db7237c/rpcs3/Emu/System.cpp#L1813-L1863)
