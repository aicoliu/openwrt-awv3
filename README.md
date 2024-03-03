can_gateway_4-v19.07.7

```
git clone https://github.com/zhangjinke/openwrt.git
cd openwrt
git checkout can_gateway_4-v19.07.7
./scripts/feeds update -a #更新feeds
./scripts/feeds install -a #将feeds安装到menuconfig
cp can_gateway_4_musl_diffconfig .config #应用配置
make defconfig #扩展完整配置
time make download V=s #下载所有依赖
time make V=99 #不可用root用户编译

```
