# 环境搭建

环境搭建方式有很多种，这里选择最简单的一种方式。

## Mac

官方直接下载pkg安装包: <https://go.dev/dl>，mac版本因为有amd和arm芯片，所以注意选择你的电脑对应的包。

```shell
go1.20.6.darwin-amd64.pkg # intel芯片
go1.20.6.darwin-arm64.pkg # arm芯片，M1, M2
```

## Linux

`linux` 下系统的包管理系统如`yum`，`apt-get` 这种提供的 `go` 包版本一般都不是最新的，如果希望安装最新版本的包，还是手动安装：

```shell
wget https://go.dev/dl/go1.20.6.linux-amd64.tar.gz 
tar -C /usr/local -xzf go1.20.6.linux-amd64.tar.gz

# 配置环境变量
vim ~/.bashrc
export PATH=$PATH:/usr/local/go/bin
source ~/.bashrc
```

## Windows

官方下载 .msi 安装包

```shell
go1.20.6.windows-386.msi
```

> 不建议在 `windows` 下本地开发 `Go`, 如果是 `Windows`系统，可以建议使用`IDE`配合虚拟机使用远程编译运行模式开发！！
