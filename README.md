# zxmake-mirror

Toolchain mirrors for CI. Create a release to trigger downloads and uploads.

## Assets

| Workflow | Files |
|----------|-------|
| ARM GNU | `arm-gnu-toolchain-{version}-x86_64-{target}.tar.xz` |
| Android NDK | `android-ndk-{version}-linux-x86_64.zip` |
| Zig | `zig-linux-x86_64-{version}.tar.xz` |

## Usage

```bash
https://github.com/TOMO-CAT/zxmake-mirror/releases/download/<tag>/<filename>
```

## Create Release

```bash
git tag <tag> && git push origin <tag>
```

Push tag 后自动触发 workflow 创建 release 并上传所有工具链。
