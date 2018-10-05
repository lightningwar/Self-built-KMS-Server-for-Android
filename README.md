# Self-built-KMS-Server-for-Android
### 作用
` 激活 Windows 系统、激活 office 全套 `
### 支持版本
[Supportted Version](https://raw.githubusercontent.com/lightningwar/Self-built-KMS-Server-for-Android/master/Supportted%20Version.txt)
### 如何下载最新版本的 Windows ISO 文件
- Chrome
- [Windows10最新版微软官方下载地址](https://www.microsoft.com/zh-cn/software-download/windows10ISO/)
- F12 → DevTools → More Tools → Networks conditions → Unchecked Select automatically → Chrome-Mac
- Then you can download the latest version.

### Windows 激活方法
- 打开 命令提示符(管理员)
- 查看系统版本
```bash
wmic os get caption
```
- 查看激活详情
```bash
slmgr /dlv
```
- 卸载密钥
```bash
slmgr /upk
```
- [KMS 客户端微软安装密钥](https://docs.microsoft.com/en-us/windows-server/get-started/kmsclientkeys)
- 在 Android 手机安装 [KMS-Server-Client.apk](https://github.com/lightningwar/Self-built-KMS-Server-for-Android/releases/download/v1.0/KMS-Server-Client.apk)
- 手机端接入本地局域网，启动服务器，查看服务器IP地址
- 在命令提示符(管理员)中依次键入
```bash
cscript slmgr.vbs /ipk *Product Key According to Edition*
cscript slmgr.vbs /skms *IP Address*
cscript slmgr.vbs /ato
```
- 成功地激活了产品

### 激活说明
>*** KMS服务是微软针对大型企业设计的激活系统，KMS批量激活密钥广泛用于机房服务器操作系统和大型企业内部批量激活员工电脑，限企业内网使用。目前公开的KMS服务器封杀力度很大，为了节省大家的时间与精力，请低调使用。 ***

>*** KMS 激活有 180 天期限，此期限称为激活有效间隔。若要保持激活状态，您的系统必须通过至少每 180 天连接一次 KMS 服务器来续订激活。默认情况下，系统每 7 天自动进行一次激活续订尝试。在续订客户端激活之后，激活有效间隔重新开始。***

>*** 综上所述，只要您的电脑不超过 180 天以上无法连接互联网，就无需进行任何操作，系统会自行续期保持激活状态。即永久激活。***
