# -ARM-
搭建ARM交叉编译化境

```shell
#下载交叉编译工具
http://snapshots.linaro.org/components/toolchain/binaries/
#选择一个版本，选择aarch64-linux-gnu，选择带有x86_64_aarch64字样的tar.xz格式压缩包

#把压缩包传入到交叉编译环境中的/opt 目录，解压压缩包
tar -xvf xxx.tar.gz

#设置环境变量，在/root/.profile下新增PATH环境变量
PATH=$PATH:/opt/xxx/bin
source /root/.profile

#修改Makefile，修改与aarch64相关的指令，要和bin目录下的一致
```

