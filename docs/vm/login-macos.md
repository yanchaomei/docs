# macOS 系统登录虚拟机

## 命令行：使用 SSH 登录 {#ssh}

macOS 自带命令行 SSH 客户端。

### 登录 {#ssh-login}

* 根据虚拟机登录 IP 地址和端口（例如，下图中地址为 `202.38.75.252`，端口为 `10004`），输入命令：

    ```shell
    ssh -p 10004 root@202.38.75.252
    ```

    此命令也可以从你的管理页面找到。

* 如果遇到 Warning，请输入 `yes`，然后输入之前设置的 root 密码，即可登录虚拟机

    ![](../images/ssh_2.png)

## 图形界面：使用 VNC 登录 {#vnc}

!!! info "注意"

    该登录方式只适用于名称中带有 `desktop` 的虚拟机镜像。

### 使用 RealVNC 登录 {#realvnc}

[下载 macOS 下的 RealVNC 客户端](https://www.realvnc.com/en/connect/download/viewer/macos/)并安装（与安装其他的应用一样，打开 dmg 文件并将应用拖动到 Application 目录即可）。

打开 VNC Viewer，打开后的主界面如图所示，在地址栏输入 `vlab.ustc.edu.cn`，按回车连接：

![RealVNC Main Screen](../images/realvnc-main-screen-macos.png)

如果出现以下画面，continue 即可。

![RealVNC Server not recognized](../images/realvnc-auth-warning-macos.png)

这里提示要输入用户名和密码，输入学号（或工号）和网页平台的登录密码即可登录：

![RealVNC Authentication Dialog](../images/realvnc-auth-screen-macos.png)

!!! question "密码是什么？"

    VNC 登录方式使用 Vlab 平台的登录密码。[还没设置？](web.md#change-password)

登录后即可看到桌面并开始使用。

### 使用 TigerVNC 登录 {#tigervnc}

[下载 macOS 下的 TigerVNC 客户端](https://vlab.ustc.edu.cn/downloads/TigerVNC-1.10.1.dmg)并安装（与安装其他的应用一样，打开 dmg 文件并将应用拖动到 Application 目录即可）。

打开 TigerVNC 客户端，如图所示输入 `vlab.ustc.edu.cn`，点击 `Connect`。

![TigerVNC Main Screen](../images/tigervnc-startup-macos.png)

这里提示要输入用户名和密码，输入学号（或工号）和网页平台的登录密码即可登录：

![TigerVNC Authentication Dialog](../images/tigervnc-authentication-macos.png)

### 桌面设置 {#desktop-settings}

关于一些常用的桌面设置，如

- 修改 VNC 分辨率
- 中文输入法

等，请参阅[桌面设置](desktop-settings.md)页面。
