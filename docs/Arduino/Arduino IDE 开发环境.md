## Arduino IDE 开发环境

**1.Windows系统：**

![Img](./media/eef95a4f71c9316e41a35813556e51da.png)

1.1. 下载安装Arduino软件：

(1)首先，进入Arduino官方网站：[https://www.arduino.cc/](https://www.arduino.cc/) ，点击“**SOFTWARE**”进入下载页面，如下图所示：

![Img](./media/09ba2def88a3782a4ea7fde0a3fa94b2.png) 

![Img](./media/3eb0ef44f14f936b8fa44bf113e4936e.png)

(2)然后，根据你的操作系统选择并下载相应的安装程序。如果你是Windows用户，请选择安装2.0.3版本Arduino IDE，当点击“**Windows** Win10 and newer,64bits”或“**Windows** MSI installer”，代表下载安装文件(.exe) ，需要手动安装; 当点击“**Windows** ZIP file”，代表直接下载2.0.3版本Arduino IDE，是一个压缩文件，解压就可以直接使用，无需安装。

![Img](./media/1f975a2153559093d34b23afd73d3e7e.png)

 点击下面图标，就可直接安装Arduino IDE了。

![Img](./media/b4fc60ff6863af3d093cd47da62f2040.png)

一般情况下，点击“**JUST DOWNLOAD**”就可以下载了，当然如果你愿意，你可以选择小小的赞助，以帮助伟大的Arduino开源事业。

(3)Arduino软件下载完成后,如果你是点击“**Windows** Win10 and newer,64bits”或“**Windows** MSI installer”下载的(.exe)文件“**arduino-ide_2.0.3_Windows_64bit.exe**” ，需要双击(.exe)文件继续安装，当你收到操作系统的警告时，请点击“**Allow access**”允许驱动程序安装。首先点击“**I Agree**”, 然后选择“Anyone who uses this computer(all users)”后再点击Next。

![Img](./media/15bcc3e3f13e89a7a3eaf2d6e9ca5b2c.png)

![Img](./media/72f9cfe86a9e89aeb3431ed66d9df5bf.png)

![Img](./media/74bde0fbec2a9a15c14435633eb7b864.png)

(4)点击“**Next**”后，如果又出现下面页面，点击“**I Agree**”。

![Img](./media/72f9cfe86a9e89aeb3431ed66d9df5bf.png)

(5)选择安装目录(我们建议保持默认目录)，然后点击“**Install**”。

![Img](./media/6c66ee9c7b948a27341de4f5d5e59ab1.png)

(6)如果出现以下界面，则应选择“**Install**”。

![Img](./media/68ddbb0c391855fd7213d5d9269eebb8.png)

该过程将提取并安装所有必需的文件，以正确执行Arduino软件(IDE)。

![Img](./media/235841a13809e8c131e0471e1c90f54a.png)

(7)安装完成后，会在桌面上生成一个Arduino IDE软件快捷方式。

![Img](./media/9152131aa663c6c5723a96c9e6f7a9a1.png)

![Img](./media/edbce928e27d6f6d26e0a6df960421da.png)

1.2. 在Windows系统上安装驱动：

（<span style="color: rgb(255, 76, 65);">注意：如果电脑已经安装了驱动程序，则不需要再安装驱动；如果没有，则需要进行以下操作</span>）
在使用ESP32主板之前，必须安装驱动程序，否则ESP32主板将无法与计算机通信。将主控板用USB线连接在电脑上，一般MacOS和Windows10系统的电脑会自动安装驱动。如果没能自动安装，则需要手动安装驱动。

（1）查看电脑是否自动安装好驱动：

点击“**计算机**”--“**属性**”--“**设备管理器**”，显示如下图是安装成功的了：

![Img](./media/65fcafd5ca192f1d566779a819e04d00.png)

（2）如果没能自动安装，那就手动安装，步骤如下：

下载CP2102驱动程序的链接：[https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads)

![Img](./media/967354bb7acd4614ce3c44b221bdfab9.png)

右键点击“**USB Serial**”，选择“**更新驱动程序(P)**”并点击。

![Img](./media/594f6af70f127b4d54239b5af7f11035.png)

跳转到以下页面，选择“**浏览我的电脑以查找驱动程序(R)**”并点击。

![Img](./media/e71e6ab23f4ecbd2c0eefb662aa50704.png)

我们在对应的文件夹中也提供有CP210X系列芯片的驱动文件，位置如下：

![Img](./media/93db967482f9b80ea98c483c8f56e498.png)

你可以先将驱动文件复制到电脑桌面上，然后点击“**浏览(R)...**”,选中CP210X系列芯片的驱动，最后点击“**下一页**”。

![Img](./media/c6fd62ecfbcc250b725abdc72f075f0c.png)

过一会儿，驱动安装成功。

![Img](./media/f7439196fa8567c300f0f3e35e399d42.png)

这个时候再打开计算机设备管理器，就可以看到CP2102驱动程序已经安装成功了，刚刚那个黄色的感叹号不见了。

![Img](./media/65fcafd5ca192f1d566779a819e04d00.png)

1.3. Arduino IDE工具栏介绍：

点击电脑桌面上的图标![Img](./media/2aa3f7ff09ff5841f1864c521af61cbd.png)，打开Arduino IDE。

![Img](./media/29c35817885841cbbc9385b4c8544290.png)

![Img](./media/752c9d4cfd38937d8b7ac496bf66d96d.png) -- 用于检查是否存在任何编译错误。

![Img](./media/84910ad669ba1c2669ec402831fbf46d.png) -- 用于将程序上传到Arduino板。

![Img](./media/8d72475c82afbebb1edf0f1fc12da524.png) -- 用于编写程序时的单步调试。

![Img](./media/c5e52211c8c8b64345c420211a2fd2ee.png) -- 用于从板接收串行数据并将串行数据发送到板的串行监视器。

![Img](./media/f97189a9ca8ff237dc41194ed5c28188.png) -- 用于串口接收的数据转换成动态曲线图。

![Img](./media/4f1db32e023aa9d575b641cd83f93b38.png) -- 用于打开最近保存的示例草图。

![Img](./media/f33fa6565913b109c0111e39340ad201.png) -- 用手动安装开发板。

**语言切换功能：**

（1）单击“File”→“Preferences”，在 Preferences 页面中将语言“English”切换成“简体中文”，点击“OK”就可以了。

![Img](./media/d44b87180f422631e697fea296cd5582.png)

![Img](./media/d77dd3ef192740d9e3d321ea94eaa105.png)

![Img](./media/9f65a26855c17f2e34252ffab28c51d7.png)


1.4. 在Arduino IDE上安装ESP32：

上面已经学习了怎么下载ArduinoIDE和怎么安装驱动，那下面就要在Arduino IDE上安装ESP32，请执行以下步骤：

<span style="color: rgb(255, 76, 65);">特别注意：你需要Arduino IDE 1.8.5或更高版本才能在其上安装ESP32。</span>

(1)点击电脑桌面上的图标![Img](./media/2aa3f7ff09ff5841f1864c521af61cbd.png)，打开Arduino IDE。

![Img](./media/e50b14820c3bb291108dc8b9c0c12843.png)

(2)点击“文件” →“首选项”，如下图：

![Img](./media/339b8fc0220890b15cac94e7fefd8e7f.png)

(3)打开下图标出的按钮。

![Img](./media/dd6d3ea8b8ab77977ff2b2af74dbcdab.png)

(4)将这个地址：https://espressif.github.io/arduino-esp32/package_esp32_index.json ，复制粘贴到里面去再点击“**确定**”保存这个地址，如下图：

![Img](./media/0f4697f40d0e4c73cdaa36a15034e63b.png)

(5)再点击“**确定**”。

![Img](./media/11dd827f1f17588419bf7be03a47211d.png)

（6）先点击“**工具**”→“**开发版:**”，，再点击“**开发版管理器...**”进入“**开发版管理器**”页面，在文本框中输入“**esp32**”，选择 <span style="color: rgb(255, 76, 65);">1.06</span> 版本进行安装，安装包不大，点击“**安装**”开始安装相关安装包。如下图：**<span style="color: rgb(255, 76, 0);">（特别提醒：选择更高版本或最新版本，可能会出现安装失败。）</span>**


![Img](./media/486d22dca3d5007c0866fe0dd4b3075e.png)

![Img](./media/fe7700b0fc213248a7b2d09cd6fc20ae.png)

![Img](./media/26766efa26cbdaa8d507e52e40317158.png)

（7）点击“**工具**”→“**开发版:**”，就可以看到安装好的ESP32 Arduino，你可以在里面查看到各种不同型号ESP32开发板，选择对应的ESP32开发板型号。

![Img](./media/7d924f3a05df1addfd61d26a4b1f9eff.png)

![Img](./media/07bbc456b0cfb6f5393701025233b38b.png)

（8）设置好板型后，再选择正确的COM口（安装驱动成功后可看到对应COM口），设置如下图。

![Img](./media/65fcafd5ca192f1d566779a819e04d00.png)

![Img](./media/2cdb1757b32b480e3dac16aa8385e13c.png)

![Img](./media/3270b2614818b728fb3fdd4a45d239f9.png)

**2.Mac系统:**

![Img](./media/a94b5505840316715e4bc9badd0421ba.png)

2.1.下载安装Arduino IDE:

进入Arduino官方网站：https://www.arduino.cc/ ，点击“**SOFTWARE**”进入下载页面，如下图所示：

![Img](./media/2f1dce89630be8f6fdd23f38ab7097ec.png)

2.2.如何安装CP2102驱动程序：

（注意：如果已经安装了驱动程序，则不需要再安装驱动；如果没有，则需要进行以下操作）
（1）用USB线将ESP32主板连接到你的MacOS系统电脑上，并打开Arduino IDE。

![Img](./media/a694cc7590112b9becc48e0ad33588ea.png)

（2）CP2102驱动下载链接：[https://cn.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads](https://cn.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads)

（3）点击下载MacOS 版本。

![Img](./media/a369c4f935f32560b84a9b3b756c7dc5.png)

（4）解压下载好的压缩包。

![Img](./media/43f7535e76478fc4bd3b4f7eb68ee068.png)

（5）打开文件夹，双击“SiLabsUSBDriverDisk.dmg”文件。

![Img](./media/e339ed4aa5a59a7ffbd426da57cc5522.png)

可以看到以下文件。

![Img](./media/ba80c239c55f073ad212e110898c9be5.png)

（6）双击“Install CP210x VCP Driver”，勾选“Don’t warn me when opening application on this disk image”并单击“Open”。

![Img](./media/b90f9fec981a67e60d6d973049c8480a.png)

（7）单击“Continue”。

![Img](./media/e3d154346714057c76f44a429d30bc75.png)

（8）先点击“Agree”，然后点击“Continue”。

![Img](./media/df1b62568fc2737d10bebe86364d6240.png)

（9）继续点击“Continue”，然后输入你的用户密码

![Img](./media/8d5943e9f17648b7b345f2cb921835e8.png)

![Img](./media/d5caae5575fc94e8837daad3675dd164.png)

（10）选择“Open Security Preferences”。

![Img](./media/36fe00477b7e98da6cd3f7d4e074c489.png)

（11）点击安全锁，输入你的用户密码来授权。

![Img](./media/4889cc38b37c1df851c7772aa1f74fe4.png)

![Img](./media/85556fc015cdb38f51375ace1c498585.png)

（12）看到锁被打开了，点击“Allow”。

![Img](./media/bb9213f09221a88dee06bd4ff792cd4c.png)

（13）回到安装界面，根据提示等待安装.

![Img](./media/d49cc02c9a101542bb4a8572da600dfe.png)

（14）安装成功

![Img](./media/dead537234a8ea1a9feab59bc451eebb.png)

2.3. 在Arduino IDE上安装ESP32：

上面已经学习了怎么下载ArduinoIDE和怎么安装驱动，那下面就要在Arduino IDE上安装ESP32，请执行以下步骤：

<span style="color: rgb(255, 76, 65);">特别注意：你需要Arduino IDE 1.8.5或更高版本才能在其上安装ESP32。</span>

(1)点击电脑桌面上的图标![Img](./media/2aa3f7ff09ff5841f1864c521af61cbd.png)，打开Arduino IDE。点击“Arduino IDE” →“首选项”，如下图：

![Img](./media/9a1550c0afb15d603b35c14fc7eb9419.png)

(2)打开下图标出的按钮

![Img](./media/2021aa4872f771da0789e9d4d35c778e.png)

(3)将这个地址：https://espressif.github.io/arduino-esp32/package_esp32_index.json ，复制粘贴到里面去再点击“**确定**”保存这个地址，如下图：

![Img](./media/01edadc223784029595d586e60336c53.png)

(4)再点击“**确定**”。

![Img](./media/f88fa3fc64d0e88254ed1f1960ff20cf.png)

（5）先点击“**工具**”→“**开发版:**”，，再点击“**开发版管理器...**”进入“**开发版管理器**”页面，在文本框中输入“**esp32**”，选择 <span style="color: rgb(255, 76, 65);">1.06</span> 版本进行安装，安装包不大，点击“**安装**”开始安装相关安装包。如下图：**<span style="color: rgb(255, 76, 0);">（特别提醒：选择更高版本或最新版本，可能会出现安装失败。）</span>**

![Img](./media/b190d9a92887ff3f38fd00f9ef6a7bc6.png)

![Img](./media/1bd7dab9f8e78713466d019451110080.png)

![Img](./media/032996f813d7ccb74e4c6c8a6a13486f.png)

（6）点击“**工具**”→“**开发版:**”，就可以看到安装好的ESP32 Arduino，你可以在里面查看到各种不同型号ESP32开发板，选择对应的ESP32开发板型号。

![Img](./media/40fb53f0ba1f781650ac404f8a25a3b6.png)

（7）设置好板型后，再选择正确的COM口（安装驱动成功后可看到对应COM口），设置如下图。

![Img](./media/b240beb6e80e99e17c399d6d65f03fb4.png)

**3.添加arduino库文件**

<span style="color: rgb(0, 209, 0); background: rgb(255, 251, 0);">特别提醒：库文件在上面 **<span style="color: rgb(255, 76, 65);">资料下载</span>** 处提供有，请下载并且安装好库文件。</span>

我们提供的Arduino库文件的路径：**..库文件\Arduino_C_Windows系统**。如下图：

![Img](./media/5684b4abc6d5bf0619f5efd62210be12.png)

3.1. Windows系统添加库文件的方法：

（1）打开Arduino IDE![Img](./media/0c8b09d3670cabd5f21d0528dd77796b.png)，在Arduino IDE界面点击“**项目**”→“**包含库**”→“**添加.ZIP库...**”。

![Img](./media/f82d63c799a10f799b43831596ea78cc.png)

（2）找到库文件存放的位置，选中对应的库文件，点击“**打开**”添加即可。库文件只能一个一个的添加。（<span style="color: rgb(255, 76, 65);">注意：库文件需要压缩为 **.ZIP格式**；这里以“**ESP32Servo-0.8.0.ZIP**”为演示，其他库文件的添加方法是一样的。</span>）

![Img](./media/857b149444929db990c7cfd142076e6e.png)

3.2. MacOS系统的库文件添加方法: 

（1）arduino IDE界面选择“**项目**” > “**包含库**” > “**添加.ZIP库...**”。

![Img](./media/bc7d51aaa2a4b4f2c3bacfc3f46ebd7f.png)

（2）找到库文件存放的位置，选中对应的库文件，点击“**打开**”添加即可。库文件只能一个一个的添加。（<span style="color: rgb(255, 76, 65);">这里以添加“ESP32Servo-0.8.0.ZIP”库文件为例，其他库文件的添加方法一样</span>），如下图：

![Img](./media/6de46c44e1866db966fcdac07b86f331.png)

到这，正常是安装成功的了。



