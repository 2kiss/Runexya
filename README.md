# Runexya 1.0.2 (Rust)

Double‑click any .exe → Proton‑GE 10–12 (fallback Experimental), always winmm=n,b, auto‑loads local DLLs (recursive, default depth=6), per‑game prefix.

## Build & Install
- sudo apt install -y cargo rustc
- cargo build --release
- chmod +x build_deb.sh && ./build_deb.sh
- sudo dpkg -i runexya_1.0.2_all.deb
- Ensure Proton‑GE is in Steam compatibilitytools.d, then restart Steam.

## Use
- Double‑click .exe or: runexya /path/to/Game.exe
- Optional: .protonge-overrides in game folder (lines like `dinput8=n,b` or `xaudio2_9=b`).
- Env:
  - DLL_DEPTH=6 (default) — change search depth
  - DISABLE_AUTO_DLL=1 — disable auto DLL scan

Prefix: ~/.local/share/runexya/compatdata/<hash>/pfx
