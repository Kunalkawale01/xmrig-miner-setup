# xmrig-miner-setup (Windows)

This repository contains the XMRig CPU miner setup for Windows 64-bit systems.

# Folder Structure

    xmrig-miner-setup/
    │
    ├── xmrig/                      # Main miner files
    │   ├── xmrig.exe
    │   ├── config.json
    │   ├── start.cmd
    │   ├── benchmark_1M.cmd
    │   ├── benchmark_10M.cmd
    │   ├── pool_mine_example.cmd
    │   ├── solo_mine_example.cmd
    │   ├── rtm_ghostrider_example.cmd
    │   ├── WinRing0x64.sys
    │   └── SHA256SUMS
    │
    ├── config/
    │   └── config.json             # Custom config file
    │
    ├── docs/
    │   └── setup-guide.md
    │
    ├── .gitignore
    ├── LICENSE
    ├── README.md
    └── requirements.md

# Features
- CPU mining support
- Benchmark mode
- Pool mining
- Solo mining
- Custom configuration support
- Requirements
- Windows 10/11 (64-bit)
- Administrator privileges
- Stable internet connection

# Installation

1.  Download the Zip :

2. Navigate to the folder:

        cd xmrig-6.25.0-windows-x64

3. Edit config.json and add your wallet address and pool.

4. Start mining:

       xmrig.exe --config config.json

# Configuration

 Edit config/config.json:
- wallet address
- mining pool
- CPU threads
