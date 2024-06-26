# XBMC/Kodi

## 镜像目录结构

| 目录 | 内容 |
| :--: | :--: |
| addons | 官方插件库 |
| apt | iOS 版 Kodi 安装源 |
| build-deps | 编译 Kodi 依赖的其他开源项目代码 |
| nightlies | 与 Kodi 开发主分支同步编译的每日开发版安装包下载目录 |
| releases | Kodi 稳定版安装包下载目录（含 Beta 版和 RC 版） |
| snapshots | Kodi 每月发布的 Alpha 版安装包下载目录 |
| tools | Kodi 相关的工具软件（Kora 遥控软件） |

## Kodi 简介

Kodi（前身是 XBMC）媒体中心，是一个屡获殊荣的自由和开源的跨平台媒体播放器和用于 HTPC（Home theater PC，家庭影院 PC）的数字媒体娱乐中心软件。它使用遥控器作为主输入设备，针对 3 米左右观看距离而设计的用户界面，成为适应客厅使用的媒体播放器。它的图形用户界面让用户轻按遥控，就能方便地从硬盘、光盘、局域网和互联网浏览和观看视频、图片，收听广播和音乐。Kodi 项目由非营利的 XBMC 基金会管理，并由分布在世界各地的志愿者参与开发。自从它于 2003 年诞生以来，超过 500 名软件开发人员对 Kodi 作出贡献，并有 60 名核心开发人员。另外，还有 200 多名翻译人员在帮助它扩大影响范围，使它支持多达 72 种语言。

Kodi（当时叫「Xbox Media Center」）最初是作为第一代 Xbox 游戏机（现在已不支持）的一个媒体中心应用而开发的，而现在已经正式以原生应用运行于 Android、Linux、Mac OS X、iOS 和 Windows 操作系统，并支持主流的处理器架构。

## 使用说明

### Kodi 安装

#### Windows、Android 平台

从镜像站相应目录下载你所需要版本的安装包安装即可。

#### Mac OS X 平台

从镜像站相应目录下载 `.dmg` 磁盘镜像文件，在 OSX 系统下装载此镜像文件后，可用鼠标将 Kodi 应用拖到「应用」文件夹即完成安装。

#### iOS 平台

需要先越狱，然后通过 Cydia 安装。

- 第一步：在已越狱的 iPhone 手机或 iPad 主屏幕上点击 Cydia 图标
- 第二步：选择"软件源 → 编辑 → 添加"
- 第三步：在弹出的录入框输入 `http://mirrors.ustc.edu.cn/xbmc/apt/ios/`
- 第四步：点击刚增加的 teamKodi 源
- 第五步：选择安装 Kodi-iOS

### 插件库使用

可以使用此镜像服务器来访问 Kodi 官方插件库，避免因网络访问的问题而无法正常安装使用插件。需要编辑 Kodi 安装目录中的 addons/repository.xbmc.org/addon.xml 文件。将其中所有 `http://mirrors.kodi.tv/` 替换为 `http://mirrors.ustc.edu.cn/xbmc/`。

### 编译依赖项目下载

开发人员或者想自行从源代码编译 Kodi 的，可以使用此镜像服务器下载依赖项目。方法是在运行 `DownloadBuildDeps.bat` 批处理文件前先在命令行执行
`SET KODI_MIRROR=http://mirrors.ustc.edu.cn/xbmc/`。

## 相关链接

Kodi 链接

- Kodi 主页：<http://kodi.tv/>
- 文档：<http://kodi.wiki/>
- Bug Tracker: <http://trac.kodi.tv/>
- 源代码：<https://github.com/xbmc/xbmc>
