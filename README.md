# wxpython-wheels

Mirror of prebuilt wxPython wheels from extras.wxpython.org/wxpython.org snapshot-builds, used by PixelFlasher CI (extras.wxpython.org is very slow/unreliable).

Releases are tagged per platform: `ubuntu-22.04`, `ubuntu-24.04`. Only Python 3.13 (cp313) Linux wheels are mirrored.

## Update process
1. `wget -c https://extras.wxpython.org/wxPython4/extras/linux/gtk3/<ubuntu>/wxpython-<ver>-cp313-cp313-linux_x86_64.whl` (or copy from a previous local download)
2. Add the file to the matching release via the web UI or `gh release upload <tag> <file> --repo badabing2005/wxpython-wheels`
3. Keep old versions; bump the version pinned in PixelFlasher workflows only after verifying the build.