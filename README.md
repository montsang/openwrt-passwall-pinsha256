# openwrt-passwall-pinsha256
Thos Version is Modified for hysteria2 user, myself of course, with a different package name: luci-app-passwall-pinsha256.
There's a compiled *.ipk in release which have the same package name with the original one.
Please install with --force-overwrite behind if you already installed.

A commonly used proxy toolchain for Openwrt LuCI Application.

## How to use
1. add new line to openwrt feeds
```
echo "src-git passwall_packages https://github.com/xiaorouji/openwrt-passwall-packages.git;main" >> "feeds.conf.default"
echo "src-git passwall https://github.com/xiaorouji/openwrt-passwall.git;main" >> "feeds.conf.default"
```
2. pull upstream commits
```
./scripts/feeds clean
./scripts/feeds update -a
./scripts/feeds install -a
```

## Note

### ⚠ Need golang version [1.20](https://github.com/openwrt/packages/tree/openwrt-23.05/lang/golang) to or higher to compile Sing-box and hysteria
