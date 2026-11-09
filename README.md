# GlassOS

GlassOS is a Debian 13 (Trixie) Live ISO project with a macOS-inspired KDE Plasma desktop.

## Included in this initial build
- Debian 13 Trixie base, amd64
- KDE Plasma desktop with SDDM
- Cairo-Dock configured to start automatically
- Firefox ESR, selected as the preferred browser
- Plymouth graphical boot splash (Debian spinner theme)
- Everyday applications: Thunderbird, LibreOffice, GIMP, Krita and VLC

## Build the ISO on GitHub (no local multi-gigabyte toolchain)
1. Open the **Actions** tab.
2. Select **Build GlassOS ISO**.
3. Click **Run workflow**.
4. Wait for the job to finish.
5. Open the successful run and download the **GlassOS-live-amd64** artifact.

A push to `main` that changes build files also starts the workflow automatically.

## Important
This is a Debian Live customization, not a new Linux kernel or an independent distribution. The first GitHub Actions build must complete successfully before an ISO exists. Review the build log if package names or upstream repositories change.

The ISO will be larger than the source configuration because it contains a desktop environment and applications.
