# OpenWrt知识点
了解和记录OpenWrt相关知识点，总结

更多详细的描述，可以参考官网：https://openwrt.org/

## 1. 简介
## 2. 文件框架

编译之前：

| File Name | Explaination                                                 |
| --------- | ------------------------------------------------------------ |
| tools     | 主机编译时需要使用的工具，含Makefile/patch等，Makefile末尾的$(eval $(call HostBuild))表征主机使用 |
| toolchain | 交叉编译工具链，含binutils/debugger/compiler等               |
| include   | OpenWrt需要的Makefile                                        |
| target    | 目标板的信息                                                 |
| scripts   | 脚本                                                         |
| package   | 编译的package                                                |

编译之后新增以下目录：	

| File Name    | Explaination                                                 |
| ------------ | ------------------------------------------------------------ |
| bin          | 生成的各种.bin文件，firmware/ipkg都会存放于此目录，bin/<platform\>/package |
| tmp          |                                                              |
| dl           | 编译时需要下载的各种源码，压缩文件                           |
| building_dir | 编译代码的目录                                               |
| staging_dir  |                                                              |

## 3. 搭建方法



## 4. 实例

## 5. 文件系统（overlay）