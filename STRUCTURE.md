# Orbit-OS Repository Structure

```
Orbit-OS/
├── bootloader/              # U-Boot and boot configuration
│   ├── uboot/              # U-Boot source (RK3126C specific)
│   └── configs/            # Boot configurations
├── kernel/                 # Linux kernel for M17
│   ├── arch/              # Architecture-specific (ARM)
│   ├── drivers/           # Device drivers
│   └── configs/           # Kernel configuration files
├── android/               # Android 4.4 KitKat system
│   ├── frameworks/        # Android framework (stripped)
│   ├── system/            # System binaries and libraries
│   ├── packages/          # System packages and apps
│   └── bionic/            # C library
├── apps/                  # Pre-installed applications
│   ├── launcher/          # Home screen launcher
│   ├── settings/          # Settings app
│   ├── files/             # File manager
│   ├── playstore/         # Play Store (lightweight)
│   └── minecraft/         # Minecraft PE v0.14.0
├── device/                # M17 device tree and configs
│   ├── rockchip/         # Rockchip (RK3126C) specific
│   ├── device_tree/      # Device tree binaries
│   └── overlays/         # Board overlays
├── build/                 # Build system and scripts
│   ├── Makefile          # Main build script
│   ├── build.sh          # Build automation
│   ├── extract_img.sh    # Image extraction script
│   └── configs/          # Build configurations
├── tools/                 # Development tools
│   ├── img_flasher.sh    # SD card flashing script
│   └── optimization/     # RAM/memory optimization scripts
├── docs/                  # Documentation
│   ├── BUILD.md          # Build guide
│   ├── DEVELOPMENT.md    # Development setup
│   ├── HARDWARE.md       # M17 hardware specs
│   └── CONTRIBUTING.md   # Contribution guidelines
├── patches/               # Custom patches for Android 4.4
│   ├── memory/           # RAM optimization patches
│   ├── kernel/           # Kernel patches
│   └── system/           # System patches
└── .github/              # GitHub configuration
    ├── ISSUE_TEMPLATE.md
    └── workflows/        # CI/CD workflows
```

## Directory Descriptions

| Directory | Purpose |
|---|---|
| `bootloader/` | Boot sequence, U-Boot for RK3126C |
| `kernel/` | Linux kernel source and configs |
| `android/` | Stripped Android 4.4 framework and core |
| `apps/` | Pre-installed and essential apps |
| `device/` | M17-specific device tree and hardware config |
| `build/` | Build scripts and system |
| `tools/` | Utilities for flashing, optimization |
| `docs/` | All documentation |
| `patches/` | Custom modifications to Android/kernel |
| `.github/` | GitHub workflows and templates |
