# ArchWSL开发环境配置

## 1. 安装ArchWSL
1. 下载 [github](https://github.com/yuk7/ArchWSL/releases) zip 安装包。
2. 解压缩 zip 文件中的全部内容到相同的目录。 请解压到一个你拥有写权限的目录。 例如， C:\Program Files 就不该被使用。
3. 运行 Arch.exe 来安装 rootfs 和注册表配置。另外，EXE 文件的名称会同时用作你的 WSL 实例名称。也就是说，如果复制多个 EXE 文件，并重命名成不同的名称，你就同时拥有了多个不同的 ArchWSL 并且互不冲突。

## 2. 配置开发环境
1. 将WSL安装目录添加到 win10 环境变量
![](https://raw.githubusercontent.com/hongcn5/image/main/ArchWSL_setup.png)

## 3. arch(x).exe用法
```
用法 :
    <无参数>
      - 以你的默认设置打开一个新的Shell。

    run <命令行>
      - 在此实例中运行你所给出的命令，继承当前Shell的所在目录。

    runp <命令行 (包含 windows 路径)>
      - 在此实例里运行转译过的命令行。

    config [setting [值]]
      - `--default-user <用户>`: 设定此实例的默认用户到 <用户>。
      - `--default-uid <uid>`: 设定此实例的默认用户 UID 到 <uid>。
      - `--append-path <on|off>`: 加入 Windows PATH 到 $PATH 的开关。
      - `--mount-drive <on|off>`: 挂载驱动器的开关。
      - `--default-term <default|wt|flute>`: 设置默认的终端窗口样式。

    get [setting]
      - `--default-uid`: 输出此实例的默认用户UID。
      - `--append-path`: 输出”加入 Windows PATH 到 $PATH“的开关状态。
      - `--mount-drive`: 输出”挂载驱动器”的开关状态。
      - `--wsl-version`: 输出此实例的WSL版本（1/2）。
      - `--default-term`: 输出此实例启动器的默认终端样式。
      - `--lxguid`: 输出此实例的 WSL GUID key。

    backup [contents]
      - `--tar`: 输出 backup.tar 到当前目录。
      - `--reg`: 输出设置注册表文件到当前目录。

    clean
      - 卸载此实例。

    help
      - 显示此帮助信息。
```

## 4. ArchWSL 初始配置
