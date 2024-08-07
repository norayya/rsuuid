# rsrand
A simple random string generator!

一个随机字符生成器。

方便在无网络非编程环境下生成使用随机字符。

目前支持UUID，其他功能后续更新。

## 使用
### 生成UUID
``` 
// rsrand uuid [new]  
// 不使用-c / --count 指定生成数量, 默认生成1个
rsrand uuid new

// rsrand uuid [new] [-c] [count]
rsrand uuid new -c 2
```

### 验证字符串是否为合法v4 UUID
```
// rsrand uuid [try] [-u] [uuid string]
rsrand uuid try -u 58667344-0503-44ea-a1be-eebdb61520c9

@:~/# success
```

---

## 安装
### Windows
* 直接使用二进制包, 在命令行中使用
* 下载源码，使用cargo本地编译

在生成目录下运行install.ps1可以将当前目录加入环境变量，重启powershell后即可以在任意目录中使用rsrand命令启动

可以运行uninstall.ps1从环境变量中卸载当前路径


### Linux
* 下载源码，使用cargo本地编译

编译后需自行软链接到二进制程序文件
```
ln -s (生成结果路径)/rsrand /usr/local/bin/rsrand
```
---

#### 一些有用的链接

[安装rust (rustc, cargo)](https://www.rust-lang.org/tools/install)

[What is UUID?](https://en.wikipedia.org/wiki/Universally_unique_identifier)

