# COMMAND

```
mkdir -p ~/openwrt
mkdir -p ~/openwrt/package
mkdir -p ~/openwrt/package/utils
mkdir -p ~/openwrt/package/utils/shc

cd ~/openwrt

wget https://raw.githubusercontent.com/mglphreaker/mglopenwrt/main/shc_openwrt.zip

unzip shc_openwrt.zip

mv shc_openwrt ~/openwrt/package/utils/shc/

make menuconfig # -> utilities -> [*]shc

make package/utils/shc/compile V=s

shc -v
```

done
