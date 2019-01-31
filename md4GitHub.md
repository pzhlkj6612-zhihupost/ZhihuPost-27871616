![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-527a03e73899862b1da8a2a3beb5a990.jpg)

禁止转载。

禁止转载是指“禁止转载本文内容”，可以通过超链接的方式分享本文。

<br/>

本文章内容由我在该问题下的回答总结而来：

[https://www.zhihu.com/question/19786618](https://www.zhihu.com/question/19786618)

本文章也存在于 GitHub 仓库：

[https://github.com/pzhlkj6612/ZhihuPost-27871616](https://github.com/pzhlkj6612/ZhihuPost-27871616)

<br/>

注意：

* 你首先应该阅读 [.NET Framework 安装指南 | Microsoft Docs](https://docs.microsoft.com/zh-cn/dotnet/framework/install/)，这是最权威的内容；
* 当你自己没法解决的时候，请求助于身边有空的、懂电脑的人；
* 以下内容有难度。

----

# 目录

- [目录](#%E7%9B%AE%E5%BD%95)
- [我需要哪些版本的 .NET Framework](#%E6%88%91%E9%9C%80%E8%A6%81%E5%93%AA%E4%BA%9B%E7%89%88%E6%9C%AC%E7%9A%84-net-framework)
- [.NET Framework 版本和依赖关系](#net-framework-%E7%89%88%E6%9C%AC%E5%92%8C%E4%BE%9D%E8%B5%96%E5%85%B3%E7%B3%BB)
- [我该如何安装 .NET Framework](#%E6%88%91%E8%AF%A5%E5%A6%82%E4%BD%95%E5%AE%89%E8%A3%85-net-framework)
- [安装 .NET Framework 4](#%E5%AE%89%E8%A3%85-net-framework-4)
- [.Net Framework 4.7 相关](#net-framework-47-%E7%9B%B8%E5%85%B3)
- [在 Windows 10、Windows 8.1 和 Windows 8 上安装 .NET Framework 3.5](#%E5%9C%A8-windows-10windows-81-%E5%92%8C-windows-8-%E4%B8%8A%E5%AE%89%E8%A3%85-net-framework-35)
- [关于错误 0x800F081F、0x800F0906、0x800F0907（复杂）](#%E5%85%B3%E4%BA%8E%E9%94%99%E8%AF%AF-0x800f081f0x800f09060x800f0907%E5%A4%8D%E6%9D%82)
- [关于错误 0x800F0922](#%E5%85%B3%E4%BA%8E%E9%94%99%E8%AF%AF-0x800f0922)
- [其他（杂乱）](#%E5%85%B6%E4%BB%96%E6%9D%82%E4%B9%B1)

----

# 我需要哪些版本的 .NET Framework
[https://docs.microsoft.com/dotnet/framework/get-started/system-requirements#supported-client-operating-systems](https://docs.microsoft.com/dotnet/framework/get-started/system-requirements#supported-client-operating-systems)

* Windows 10 1809 已预装 4.7.2，可以安装 3.5；
* Windows 10 1803 已预装 4.7.2，可以安装 3.5；
* Windows 10 1709 已预装 4.7.1，可以安装 3.5；
* Windows 10 1703 已预装 4.7，可以安装 3.5 和 4.7.2；
* Windows 10 1607 已预装 4.6.2，可以安装 3.5 和 4.7.2；
* Windows 10 1511 已预装 4.6.1，可以安装 3.5 和 4.6.2；
* Windows 10 1507 已预装 4.6，可以安装 3.5 和 4.6.2；
* Windows 8.1 已预装 4.5.1，可以安装 3.5 和 4.7.2；
* Windows 8 已预装 4.5，可以安装 3.5 和 4.6.1；
* Windows 7 SP1 已预装 3.5.1，可以安装 4.7.2；
* Windows XP 没有预装 .NET Framework，可以安装 3.5 和 4.0。

注意：

* 对于 .NET Framework 4.X，如果上述的某版本无法在你的系统上安装，请尝试安装更低的版本，直到安装成功。如果到 4.0 都没有安装成功，请重装系统。
* Windows 7 不是 SP1 请尽快升级，参考：[https://support.microsoft.com/help/15090](https://support.microsoft.com/help/15090)
* 除非有必要，不建议继续使用 Windows XP。

<br/>

<br/>

# .NET Framework 版本和依赖关系
[https://docs.microsoft.com/dotnet/framework/migration-guide/versions-and-dependencies](https://docs.microsoft.com/dotnet/framework/migration-guide/versions-and-dependencies)

> ... 每个新版本的 .NET Framework 都会保留早期版本中的功能并会添加新功能。 CLR 由其自己的版本号标识。 虽然 CLR 版本并不总是递增的，但 .NET Framework 版本号在每次发布时都会递增。 例如，.NET Framework 4、4.5 和更高版本包含 CLR 4，而 .NET Framework 2.0、3.0 和 3.5 包含 CLR 2.0。 （没有版本 3 的 CLR。）

[CLR](https://docs.microsoft.com/dotnet/standard/clr) - **C**ommon **L**anguage **R**untime

<br/>

<br/>

# 我该如何安装 .NET Framework

* 对于 .NET Framework 4.X，请参考“安装 .NET Framework 4”部分；

* 对于 .NET Framework 3.5，请参考“在 Windows 10、Windows 8.1 和 Windows 8 上安装 .NET Framework 3.5”部分。

<br/>

<br/>

# 安装 .NET Framework 4

当你运行的程序需要 .NET Framework 4.0 及以上版本的环境，但当前系统中并没有时，会报错：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-630dcba5364d2845bb2e7fe94fb0e13d.jpg)

去这里下载安装程序：[https://docs.microsoft.com/dotnet/framework/install/guide-for-developers](https://docs.microsoft.com/dotnet/framework/install/guide-for-developers)

<br/>

<br/>

# .Net Framework 4.7 相关

由于在 Windows 7、 Windows Server 2008 R2 和 Windows Server 2012 中可能缺少 D3DCompiler_47.dll，4.7 的安装会失败：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-50c47193ff28963e90d09057b46da372.jpg)

解决方法：打上对应操作系统版本的 KB4019990；

详细信息：[https://support.microsoft.com/help/4020302](https://support.microsoft.com/help/4020302)

打上补丁后：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-36663f1ec4b9c9fe1de7be1caa1550d8.jpg)

另外，安装 4.7 时最好确保你的系统有一个稳定的 Internet 连接，不然可能会遇到错误：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-415656a93a19877065b52df9e9ed6277.jpg)

相关参考（未验证）：

* [http://technet.microsoft.com/library/dn265983.aspx](http://technet.microsoft.com/library/dn265983.aspx)
* [http://blog.csdn.net/bokutake/article/details/50058763](http://blog.csdn.net/bokutake/article/details/50058763)

<br/>

<br/>

# 在 Windows 10、Windows 8.1 和 Windows 8 上安装 .NET Framework 3.5

微软文档库中**曾经**有过这样一句话：

> 由于安装 .NET Framework 3.5 所必须采用的方法十分复杂，很遗憾不能提供可以独立于 Windows 更新运行的单独的独立安装程序。

也就是说，你需要进行一定的操作才能把 3.5 装好，而不是下载一个安装程序那么简单。

注意：MD5 为 D481CDA2625D9DD2731A00F482484D86、大小为 231 MB 的“dotnetfx35.exe”并不是 .NET Framework 3.5 的离线安装包。

<br/>

跟着官方文档走：[https://docs.microsoft.com/dotnet/framework/install/dotnet-35-windows-10](https://docs.microsoft.com/dotnet/framework/install/dotnet-35-windows-10)

<br/>

**\* 使用系统镜像安装 .NET Framework 3.5（高级）**

这一节是对《使用部署映像服务和管理 (DISM) 部署 .NET Framework 3.5》（[https://docs.microsoft.com/windows-hardware/manufacture/desktop/deploy-net-framework-35-by-using-deployment-image-servicing-and-management--dism](https://docs.microsoft.com/windows-hardware/manufacture/desktop/deploy-net-framework-35-by-using-deployment-image-servicing-and-management--dism)）基于我个人理解、并不太准确但可以用的补充。

如果你无法连接到 Internet，或是下载进度长时间停止不前，再或者是在前述的步骤中遇到了错误，你可以尝试使用对应操作系统版本的镜像文件来安装 .NET Framework 3.5。

* 双击或右键镜像文件，选择“挂载”（或执行命令“explorer *.iso”），或解压镜像文件，找到“sources\sxs”目录；
* 按 Win+X，单击“命令提示符 (管理员)”或“Windows PowerShell (管理员)”，在命令行界面下输入以下命令，等待完成即可。

``` batch
DISM /Online /Enable-Feature /FeatureName:NetFx3 /All /LimitAccess /Source:"X:\sources\sxs"
```

（“X:\sources\sxs”是你镜像里 sources 目录下 sxs 文件夹的路径；注意要使用半角标点符号；可以不区分大小写）

下图是在 Windows 10 1803 (17134.112) 中进行的安装（使用 Shift+F10 调出 cmd；建议你在进入桌面后再进行 3.5 的安装，不要像我这样搞）：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-173976a13793484b2254d06fec499b7c.png)

<br/>

<br/>

# 关于错误 0x800F081F、0x800F0906、0x800F0907（复杂）

[https://support.microsoft.com/help/2734782](https://support.microsoft.com/help/2734782)

<br/>

终极的解决方法：重装系统。

以下是我自已测试过的情况：

* 0x800F0906
1. 由于未连接到 Internet 或用户中断了下载过程而出错；
2. 在 Windows 8 和 Windows 8.1，使用系统镜像安装 3.5 时，没有使用“/LimitAccess”参数，但指定的源路径有误，且 Windows Update 出错或未连接到 Internet 而出错；
3. 由于组策略设置出错而出错（与 0x800F0907 有所不同）。

<br/>

* 0x800F0907

组策略设置禁止。解决方法：组策略(gpedit.msc) - 计算机配置 - 管理模板 - 系统 - 制定可选组件安装和组件修复的设置，改为“未配置”或“已禁用”。

<br/>

* 0x800F081F
1. 使用系统镜像安装 3.5 时，使用了“/LimitAccess”参数，由于指定的源路径有误而出错；
2. 在 Windows 10，使用系统镜像安装 3.5 时，没有使用“/LimitAccess”参数，但指定的源路径有误，且 Windows Update 出错或未连接到 Internet 而出错；
3. 在出现过一次 0x800F081F 后，若指定的源路径不变，无论此时源路径是否正确，都会持续出现该错误。解决方法：重启系统（注销没用）。

\* 出现 0x800F081F，原因包括但不限于：路径输入错误、64 位系统指定了 32 位镜像的源（反过来同样）、源路径所属镜像所包含系统的版本号与当前系统的不等（参考：[Operating System Version](https://docs.microsoft.com/windows/desktop/SysInfo/operating-system-version) ）。

<br/>

* 0x800F081F、0x800F0906

[https://support.microsoft.com/help/3005628](https://support.microsoft.com/help/3005628)

[https://grylewicz.pl/wlaczanie-funkcji-net-3-5-i-blad-0x800f081f-w-windows-8-1/](https://grylewicz.pl/wlaczanie-funkcji-net-3-5-i-blad-0x800f081f-w-windows-8-1/)

在没有其他问题的情况下，给打过 KB2966827 的 Windows 8 和 Windows Server 2012 ，或者打过 KB2966828 的 Windows 8.1 和 Windows Server 2012 R2 第一次安装 .NET Framework 3.5 时可能会出错：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-2edc574fda1161a93716d84403ff8e46.jpg)

解决方法：打上对应操作系统版本的 KB3005628，记得要“以管理员身份运行”；

提示：KB3005628 的作用是删除 KB2966827 或 KB2966828；从 [Update for the .NET Framework 3.5 on Windows 8, Windows 8.1, Windows Server 2012, and Windows Server 2012 R2](https://support.microsoft.com/en-us/help/3005628/update-for-the-net-framework-3-5-on-windows-8-windows-8-1-windows-serv) 下载的“ndpfixit-kb3005628-XNN.exe”与 [Search results for "3005628" - Microsoft Update Catalog](https://www.catalog.update.microsoft.com/Search.aspx?q=3005628) 下载的“ndpfixit-kb3005628-xNN_\*SHA-1\*.exe”并不是同一个文件，前者运行时会弹出命令行窗口并立刻消失（不清楚是否有信息被打印出来），后者没有任何窗口，两者运行后不弹出任何提示，但一段时间后能发现 KB2966827 或 KB2966828 被删除了，看上去两者的功能是相同的。

\* 使用 Beyond Compare 简单做了个对比，可以看出“ndpfixit-kb3005628-XNN.exe”是 CLI，“ndpfixit-kb3005628-xNN_\*SHA-1\*.exe”是 GUI ，其他的区别可能就需要去做逆向之类的才能发现了：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-f12299187273f190eade4431859b9469.png)

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-1c95a3cc688d89adfd51e6ce6f656678.png)

<br/>

<br/>

# 关于错误 0x800F0922

这个错误并不仅在 .NET Framework 的安装中出现，而是一个通用的 Windows Update 错误，但你仍然可以先跟着这个教程做尝试，注意要找到“0x800F0922”那一段：[https://support.microsoft.com/help/2734782#section-2](https://support.microsoft.com/help/2734782#section-2)

不奏效的话，你还可以看着这个教程做尝试：[https://support.microsoft.com/help/10164](https://support.microsoft.com/help/10164)

还不行的话，看看 Microsoft TechNet 社区里的朋友们都做了哪些尝试，跟着试一试：[https://social.technet.microsoft.com/Forums/en-US/d689ea30-0054-4691-88df-1dac5549ffe2](https://social.technet.microsoft.com/Forums/en-US/d689ea30-0054-4691-88df-1dac5549ffe2)

也可以看看 Mobile01 论坛里的讨论：[https://www.mobile01.com/topicdetail.php?f=300&t=5542860](https://www.mobile01.com/topicdetail.php?f=300&t=5542860)、[https://www.mobile01.com/topicdetail.php?f=300&t=5540162](https://www.mobile01.com/topicdetail.php?f=300&t=5540162)。

<br/>

<br/>

# 其他（杂乱）

* 操作系统的语言包配置似乎也会影响 .Net Framework 3.5 的安装：[http://winitpro.ru/index.php/2014/10/28/oshibka-0x800f081f-pri-ustanovke-net-framework-3-5-v-windows-8-server-2012/](http://winitpro.ru/index.php/2014/10/28/oshibka-0x800f081f-pri-ustanovke-net-framework-3-5-v-windows-8-server-2012/)

<br/>

* 在 Windows 8 上即使打了 Windows8-RT-KB4019990-x64.msu，也不能安装 4.7：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-7341f6dae3d16d5a40cacc60c23193a4.jpg)

<br/>

* 在 Microsoft 官方文档中 Windows 8 最高并不支持 4.6.2，但实测可以安装：

（稳定性未知，而且我忘了具体要怎么做了）

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-8e59a1c5f099afaaeb38420b6f54e924.jpg)

<br/>

* 在 Microsoft 官方文档中 Windows Vista SP2 最高并不支持 4.6.1，但实测可以安装：

（稳定性未知）

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-4acd0223a3f291290c39dad84ed31fa7.jpg)

<br/>

* 在 Microsoft 官方文档中 Windows Vista 最高并不支持 4.7，经 [@Rayista](https://www.zhihu.com/people/abb1e9c50d0cb03b15812f503df208f6) 测试可以安装：

（稳定性未知；需要解压安装程序，运行 netfx_Full_x86.exe 或 netfx_Full_x64.exe 安装）

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-e57c6e226d1b682503147029d0c2401d.jpg)

<br/>

* 在 Microsoft 官方文档中 Windows 10 1507 最高支持 4.7，但我这边有台 Windows 10 Enterprise 2015 LTSB (10.0.10240.17488)不能安装，后来重装了系统：

（未知的原因）

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-91f4a0193012b30e59625c8f61b3c7ba.jpg)

<br/>

* 我这里测试 cn_windows_embedded_8.1_industry_pro_with_update_x64_dvd_6052079 使用 DISM 安装 3.5 会卡住，大约 20 分钟后提示失败，“错误：87；enable-feature 选项未知”：

（未知的原因，我提供了日志）

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-77984e5148f4040353f41e83f9e2c79f.png)

完成各项初次配置、进入桌面后，重新执行命令，可以成功启用 .NET Framework 3.5。检查日志文件“%SystemRoot%\Logs\dism.log”，关键内容有：
```
...
DISM Package Manager: PID=3792 TID=1516 Failed to create session classID - waiting for a second and trying again, hr:0x80080005 - CDISMPackageManager::RefreshInstanceAndLock(hr:0x80080005)
...
DISM Package Manager: PID=3792 TID=1516 Failed to create session classID - waiting for a second and trying again, hr:0x80080005 - CDISMPackageManager::RefreshInstanceAndLock(hr:0x80080005)
DISM Package Manager: PID=3792 TID=1516 Failed doing internal initialization - CDISMPackageManager::Initialize(hr:0x80080005)
DISM Provider Store: PID=3792 TID=1516 Failed to call Initialize method on IDismServicingProvider Interface - CDISMProviderStore::Internal_LoadProvider(hr:0x80080005)
DISM Provider Store: PID=3792 TID=1516 Failed to Load the provider: C:\Windows\TEMP\ECE1AB77-A6EB-47DB-AF5B-594D79ED8397\CbsProvider.dll. - CDISMProviderStore::Internal_GetProvider(hr:0x80080005)
...
DISM.EXE: No providers were found that support the command(enable-feature). HRESULT=80070057
...
```

完整日志请查看 [dism.log](./src/dism.log)，包含在完成各项初次配置、进入桌面前安装失败的和进入桌面后安装成功的所有内容。

类似的问题：[MSU Fails to install with DISM.exe error 87 - Developer Community](https://developercommunity.visualstudio.com/content/problem/31784/httpsakamsvssetuperrorreportsqpackageidmicrosoftwi.html)

<br/>

* 这里还有更多的问题：[Win8.1无法安装.NET Framework 3.5的解决办法【windows8吧】_百度贴吧](http://tieba.baidu.com/p/3647366816)

---

[@大维克多](https://www.zhihu.com/people/fb7e493cc7006f6bd91161e845962c77) 协助，

[@Wang Chunwei](https://www.zhihu.com/people/3b05b1aa0b80b69dafd6174db94e642b) 、 [@Radow](https://www.zhihu.com/people/e8db6f4700f18306f820c4184452aff1) 指正，

[@远方的记忆](https://www.zhihu.com/people/0b75516aae2a68714c7affb6a2b49984) 提示，

[@Rayista](https://www.zhihu.com/people/abb1e9c50d0cb03b15812f503df208f6) 补充，

[@李夏熙](https://www.zhihu.com/people/a580603e1238b809fcee7b643034d3fe) 提供 0x800F081F 错误信息：

![](https://raw.githubusercontent.com/pzhlkj6612/ZhihuPost-27871616/master/pic_zhimg_com/v2-0315cf4474c4a6f0728e9edc7d5b0dd2.jpg)

[@傅经纬](https://www.zhihu.com/people/c6e2b7029aa83e40e5003a5c16af7181) 提供 0x800F0922 错误信息，且网络上有相似问题，

[@墨子 2200MHz](https://www.zhihu.com/people/faf758840a7dfc528c4f620cdddf1460) 整理。

<br/>

原答案发布于：2016.05.20

原答案修改于：2017.07.14

<br/>

发布于：21:40 2017/07/13

修改于：23:46 2019/01/31

禁止转载。
