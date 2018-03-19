# minieap for OpenWRT

## Build

First download [OpenWRT SDK](https://downloads.openwrt.org/) for your device.

```sh
cd /path/to/your/sdk
git clone https://github.com/GZHU-Dress/openwrt-minieap.git package/minieap
make menuconfig # choose `minieap` in section `Network`
make package/minieap/compile V=s
```
使用方法：sudo ./minieap -u 账号 -p 密码 -n 网卡名 -d1 --module rjv3
经过测试不能心跳，但是可以掉线重新认证
