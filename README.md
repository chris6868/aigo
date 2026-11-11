# SXMonitor for Intel macOS

爱国者 冰魄 SX系列水冷mac版驱动

## 📖 使用方法

1. 保存整个 ZIP 到 U 盘、移动硬盘或其他备份位置。<br/>
2. 重装 macOS 后解压，双击 SXMonitor-Intel-1.1.0.pkg。<br/>
3. 按安装向导完成安装，输入一次管理员密码。<br/>
4. 安装完成会自动启动；以后每次登录桌面自动静默运行，不弹终端。<br/>

安装包内置独立 Python，无需联网、无需安装 Python 或 Xcode。<br/>
安装完成后可以删除解压目录；请保留 ZIP 作为重装备份。<br/>
安装包会备份并停用已安装的源码版用户自启配置，保留旧源码和日志。<br/>

卸载
双击 卸载SXMonitor.pkg，按向导完成卸载。<br/>
卸载停止离线安装版并移除其程序、自启配置，保留用户日志和旧版源码。<br/>
卸载后不会自动重新启用已备份的旧版自启配置。<br/>

适用环境
仅 Intel macOS 10.15 或更新版本，不支持 Apple 芯片。<br/>
屏幕 USB 数据接口为 VID 0145 / PID 1001，数据线必须连接。<br/>
沿用原有 VirtualSMC/FakeSMC 和 CPU 温度传感器（通常需要 SMCProcessor）。<br/>
本包不安装 EFI、驱动或传感器插件。重装时需恢复原有黑苹果驱动配置。<br/>
自启发生在登录桌面后，实际亮屏时间取决于 USB、温度传感器和屏幕固件。<br/>

安装位置
/Library/Application Support/SXMonitor/<br/>
/Library/LaunchAgents/com.sxdisplay.monitor.plist<br/>
后台日志：~/Library/Application Support/SXMonitor/monitor.log 和 error.log<br/>

包用于个人离线备份，未做 Apple Developer ID 签名或公证。<br/>
若系统拦截，确认文件来自自己的备份后，在“系统设置 → 隐私与安全性”<br/>
选择“仍要打开”（较旧系统对应“系统偏好设置 → 安全性与隐私”）。<br/>

SHA256SUMS.txt 提供两个 PKG 文件的校验值。<br/>
运行时来源、版本和校验值记录在 build-manifest.json，许可证见 licenses/。<br/>
