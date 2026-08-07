# Changelog — Kemarian fork (PocketNES)

Fork versioning: upstream date-version + `-kN` suffix, shown in the emulator
menu ("PocketNES 2025-4-16-k1 on GBA").

## 2025-4-16-k1 (2026-08-07) — branch `omega-tweaks`

- **Autosleep OFF by default** (stime=3 + matching sleeptime; menu cycle
  unchanged). Note: `stime` moved out of EWRAM_BSS — `.sbss` rejects nonzero
  initializers.
- **Build fix for devkitARM GCC 12**: removed `-finline-stringops` (GCC 13+
  flag) from `Makefile_mb`.
