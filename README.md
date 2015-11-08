![image](https://raw.github.com/Noxwizard/dnscrypt-winclient/master/screenshot.png)

About
=====
The purpose of this application is to allow the user to have a better experience controlling the DNSCrypt Proxy on Windows. It was primarily created because the proxy could not originally run in the background, so I needed a way to minimize it out of sight. It is targeted at .NET 2.0 to reach a wider audience, is built on Visual Studio 2012, and is released under the MIT license.

Requirements
============
DNSCrypt Proxy 1.4.0 or greater (http://download.dnscrypt.org/dnscrypt-proxy/)  
Microsoft .NET Framework 2.0 or greater (http://www.microsoft.com/net)

Running
=======
The necessary files can be found in the /binaries directory. Unless you have issues, use the Release files.  
Simply place the DNSCrypt proxy files in the same directory as this binary and execute the Windows client.

Required DNSCrypt Proxy files
-----------------------------
DNSCrypt 1.4.0: The contents of the /bin directory
DNSCrypt 1.6.0+: There is no longer a folder separation, just place everything in one directory

Features
========
- Enable DNSCrypt on multiple adapters via a checkbox
- Start/Stop the DNSCrypt proxy
- Enable the proxy to act as a gateway device
- Install/Uninstall/Start/Stop DNSCrypt as a Windows service
- Choose from multiple DNSCrypt providers


When launched as a standalone process and a box is unchecked or the application is closed, all DNS server settings are reverted to their original state. This is so that browsing doesn't break if the proxy isn't restarted on the next system start. The "(Automatic)" marker appears if no DNS servers were assigned and they are provided by the router/ISP.

Known Issues
============
- Does not remember custom network settings after closing when using as a service
- Cannot specify the local address to bind on
- Plugin support incomplete

Possible future plans
=====================
- Pick up a few of the other parameters that the proxy accepts
- Restore ability to add custom providers

# 中文说明
这个是 (https://github.com/Noxwizard/dnscrypt-winclient) 开源项目的分支。我主要做一些汉化工作，虽然我觉得不用汉化也很容易使用，不过还是会有些“不是中文会死星人”的。

其实这个最原始的是DNSCrypt Proxy，用来干啥你懂的，我什么都不知道，只是在自学C#罢了~

# 使用方法
上面的英文你看不懂也没关系。你只需知道，你要到 (http://download.dnscrypt.org/dnscrypt-proxy/) 下载一个叫“dnscrypt-resolvers.csv”的文件放到这个程序的根目录，然后将系统的DNS设置为 127.0.0.1 ，双击运行本程序，选择网卡，设置DNS，然后点安装、开始即可。当然，这个网站是需要科学上网的。
 
# 未来计划
除了汉化之外，为了适应国内的网络环境，我可能会添加一些功能进去。