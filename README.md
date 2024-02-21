# landv-VDI

虚拟桌面基础设施（VDI）是一种用于集中创建和管理虚拟桌面的软件工具。 虚拟桌面是模拟真实台式计算机的软件应用程序。 VDI 技术在中央服务器上创建虚拟桌面，远程用户可以通过互联网从任何实体机访问此桌面。 VDI 可快速高效地设置许多虚拟桌面，以提供对内部业务应用程序和服务的安全远程访问。

## 核心项目

以下是[jumpserver](https://github.com/jumpserver)项目，删除线部分是jumpserver未开源项目。

仅用于参看，需要使用golang全部重新实现一遍。

| 项目                                                       | 状态                                                         | 描述                                                         |
| ---------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Core](https://github.com/landv-vdi/jumpserver)           | <a href="https://github.com/landv-vdi/jumpserver/releases"><img alt="JumpServer" src="https://img.shields.io/github/release/jumpserver/jumpserver.svg" /></a> | JumpServer API 项目                                          |
| [Lina](https://github.com/landv-vdi/lina)                 | <a href="https://github.com/landv-vdi/lina/releases"><img alt="Lina release" src="https://img.shields.io/github/release/jumpserver/lina.svg" /></a> | JumpServer Web UI 项目                                       |
| [Luna](https://github.com/landv-vdi/luna)                 | <a href="https://github.com/landv-vdi/luna/releases"><img alt="Luna release" src="https://img.shields.io/github/release/jumpserver/luna.svg" /></a> | JumpServer Web Terminal 项目                                 |
| [KoKo](https://github.com/landv-vdi/koko)                 | <a href="https://github.com/landv-vdi/koko/releases"><img alt="Koko release" src="https://img.shields.io/github/release/jumpserver/koko.svg" /></a> | JumpServer 字符协议 Connector 项目                           |
| [Lion](https://github.com/landv-vdi/lion-release)         | <a href="https://github.com/landv-vdi/lion-release/releases"><img alt="Lion release" src="https://img.shields.io/github/release/jumpserver/lion-release.svg" /></a> | JumpServer 图形协议 Connector 项目，依赖 [Apache Guacamole](https://guacamole.apache.org/) |
| ~~[Razor](https://github.com/landv-vdi/razor)~~           | <img alt="Chen" src="https://img.shields.io/badge/release-私有发布-red" /> | ~~JumpServer RDP 代理 Connector 项目~~                       |
| ~~[Tinker](https://github.com/landv-vdi/tinker)~~         | <img alt="Tinker" src="https://img.shields.io/badge/release-私有发布-red" /> | ~~JumpServer 远程应用 Connector 项目 (Windows)~~             |
| ~~[Panda](https://github.com/landv-vdi/Panda)~~           | <img alt="Panda" src="https://img.shields.io/badge/release-私有发布-red" /> | ~~JumpServer 远程应用 Connector 项目 (Linux)~~               |
| ~~[Magnus](https://github.com/landv-vdi/magnus-release)~~ | <a href="https://github.com/landv-vdi/magnus-release/releases"><img alt="Magnus release" src="https://img.shields.io/github/release/jumpserver/magnus-release.svg" /> | ~~JumpServer 数据库代理 Connector 项目~~                     |
| ~~[Chen](https://github.com/landv-vdi/chen-release)~~     | <a href="https://github.com/landv-vdi/chen-release/releases"><img alt="Chen release" src="https://img.shields.io/github/release/jumpserver/chen-release.svg" /> | ~~JumpServer Web DB 项目，替代原来的 OmniDB~~                |
| [Kael](https://github.com/landv-vdi/kael)                 | <a href="https://github.com/landv-vdi/kael/releases"><img alt="Kael release" src="https://img.shields.io/github/release/jumpserver/kael.svg" /> | JumpServer 连接 GPT 资产的组件项目                           |

## TODO

- wireguard
- proxmoxve
- JumpServer(golang 重构)

使用wireguard连接JumpServer跳板机，wireguard运行在虚拟机里面，限制只能访问到跳板机。

其中跳板机主要用于审计。

跳板机系统需要实现，扫码登录+2fa双重认证(otp)

虚拟机需要实现系统还原和不还原两种功能。



