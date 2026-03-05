
## Thonny IDE 开发环境

在开始构建项目之前，你需要首先做一些准备，这是非常重要的，你不能跳过。

**一、安装Thonny(重要)：**

Thonny是一个免费、开源的软件平台，体积小，界面简单，操作简单，功能丰富，是一个适合初学者的Python IDE。在本教程中，我们使用这个IDE在整个过程中开发ESP32。Thonny支持多种操作系统，包括Windows, Mac OS,  Linux。

1.下载Thonny软件：

(1) 进入软件官网：[https://thonny.org](https://thonny.org) 下载Thonny软件，最好下载最新版的，否则可能不支持ESP32.

![Img](./media/691aee88a6f0771c7416be3547acd6ce.png)

![Img](./media/d577f429469daa3e36f0270f6f14be9c.png)

**2.Windows上安装Thonny软件：**

A.下载后的Thonny图标如下。

![Img](./media/8391c0dcc090cdbee910616f125c4a27.png)

B.双击“thonny-4.0.2.exe”，会出现下面对话框，我这里是选择“![Img](./media/b893aed32cde73b09cdb948d5588eccf.png)”进行操作的。你也可以选择“![Img](./media/86721bc54bd171a95e76e140d6216733.png)”进行操作的。

![Img](./media/25937888ff93553e85fa1d0ba89df5d8.png)

C.如果您不熟悉电脑软件安装，您可以一直单击“**Next**”直到安装完成。

![Img](./media/35cb8372fa4264fffd276a23ac041779.png)

![Img](./media/a30d1d505b110d16c3a4304108ed47fa.png)

D.如果您需要更改Thonny软件的安装路径，可以单击“**Browse...**”进行修改。选择安装路径后，单击“**OK**”。

如果您不想更改安装路径，只需单击“**Next**”；然后又继续单击“**Next**”。

![Img](./media/087d0515e40f7926c250482a352000a1.png)

![Img](./media/4d6b986f8e5e45ebf5ea981d0bd8779b.png)

E.选中“**Create desktop icon**”，Thonny软件会在你的桌面上生成一个快捷方式，方便你稍后打开Thonny软件。

![Img](./media/7e624c096b03fe4de2a81d8f45daf7a1.png)

F.单击“**Install**”安装软件。

![Img](./media/47917e20d7b062993d29c1ba485af9b1.png)

G.在安装过程中，您只需等待安装完成，千万不要点击“**Cancel**”，否则将无法安装成功。

![Img](./media/86f0178f6de6b3588bd6c5d58bcba927.png)

H.一旦看到如下界面，就表示已经成功安装了Thonny软件，点击“**Finish**”就可以。

![Img](./media/509aa2c1bbda49b81e2e5c40eae16cec.png)

I.如果你在安装过程中选择了“**Create desktop icon**”，则可以在桌面上看到如下图标。

![Img](./media/c6058db9b9639b732e8addec644f1220.png)

**二、Thonny软件基本配置**

A.双击Thonny软件的桌面图标，可以看到如下界面，同时还可以进行语言选择(<span style="color: rgb(255, 76, 65);">这里选择简体中文</span>)和初始设置。设置完了点击“**Let’s go！**”。

![Img](./media/20e07e892206f4851f5d20e48bebd4a4.png)

![Img](./media/12af365d1396796f599b6dfe30919e57.png)

![Img](./media/8efbe0a5775b66f7c79d27dc7ca196e0.png)

![Img](./media/d3ad2e747e3a8d93006bf65142c19801.png)

![Img](./media/1b36b52a8a0e036c6d42177706588dd7.png)

B.选择“**视图**”→“**文件**”和“**Shell**”。

![Img](./media/610b462833d8282fb05958d2cd6f3ec5.png)

![Img](./media/c27f1203c244e5b4b8f912a218aa2ab5.png)

![Img](./media/00a23e714ffd72f5d4fcb50bf4e5af3e.png)

**三、安装CP2102驱动：**

ESP32通过CP2102驱动下载代码。所以在使用它之前，我们需要在计算机中安装CP2102驱动程序。

**Windows 系统**

检查CP2102驱动是否已经安装

1. 用USB线连接计算机和ESP32。

![Img](./media/46cf3a8a1c79e456ac0f02da5ef38aec.png)

2. 进入计算机主界面，选择“**此电脑**”，右键单击选择“**管理**”。

![Img](./media/94d329cb6c1b4e473da1c3efaa2ff1b4.png)

3.单击“**设备管理器**”。如果你的计算机已经安装了CP2102驱动，则可以看到“**Silicon Labs CP210x USB to UART Bridge(COMx)**”。

![Img](./media/26257c4da22869d81c9a5795a3f86768.png)

安装CP2102驱动

1. 如果未安装CP2102驱动，界面显示如下。

![Img](./media/0fe123111f8eaa410a8475f9f889da21.png)

2.单击“**CP2102 USB to UART Bridge Controller**”，右键选择“**更新驱动程序(P)**”。

![Img](./media/1bb381872c77f0ea8da2f3184da164be.png)

3.单击“**浏览我的电脑以查找驱动程序(R) **”.

![Img](./media/70fb71e2b93d86b87e640ca2eb94b3ae.png)

4.单击“浏览(R)...”选择CP210x_6.7.4(驱动路径：**..\其他重要资料\CP2102驱动文件\CP2102 驱动文件-Windows**)，单击“**下一页**”

![Img](./media/684ee28b12b9f0e8e92ed402f9cfabd8.jpg)

5. 等待CP2102驱动安装完成。当界面显示如下时，表示已安装CP2102驱动。你可以关闭该界面。

![Img](./media/b2529cab7d8766c0622d14280e18b39c.png)

6.ESP32与计算机连接时，界面显示如下。

![Img](./media/dbf6accbe744c1625042c7164379a748.png)

**MAC 系统**

安装CP2102驱动方法请参照 “**<span style="background: rgb(255, 251, 0);">Arduino C 教程</span>**” 教程中 “<span style="color: rgb(255, 76, 65);">开发环境设置</span>” 部分。

**四、烧入Micropython固件(重要)**

要在ESP32主板上运行Python程序，我们需要先将固件烧入到ESP32主板。

下载Micropython固件

microPython官方网站：[http://micropython.org/](http://micropython.org/)

网页列出microPython的ESP32固件：[https://micropython.org/download/esp32/](https://micropython.org/download/esp32/)

![Img](./media/e104b567a7591c6ee38fa034c105ea67.png)

本教程中使用的固件是：<span style="color: rgb(0, 209, 0);">esp32-20210902-v1.19.bin</span>

我们的文件夹中也提供了这个固件：“**..\其他重要资料\Python固件和软件\Python_固件**”。

![Img](./media/img-20241023155948.png)

烧入Micropython固件

用USB线连接计算机和ESP32主板。

![Img](./media/46cf3a8a1c79e456ac0f02da5ef38aec.png)

确保驱动程序已成功安装，并能正确识别COM端口。打开设备管理器并展开“**端口(COM和LPT)**”。
![Img](./media/9520c883fda5ad7907b23114abf7dd34.png)

<span style="color: rgb(255, 76, 65);">注意：不同的电脑，COM端口可能不同，这是正常情况。</span>
<br>

1.打开Thonny，点击“**运行**” ，选择 “**配置解释器**”

![Img](./media/188fd4cf61083403f7d8bd9f96814814.png)

2.选中“**MicroPython (ESP32)**”，选中“**Silicon Labs CP210x USB to UART Bridge(COM7)**”，然后点击“**安装或更新MicroPython**”。

![Img](./media/33f47e1085dd98fe7a1a87c955e3fa4c.png)

![Img](./media/7553f3dadd7528fd9d0c1a493a34282c.png)

![Img](./media/3560ea7fdd94b1c9e9fc6c118d51ca3b.png)

3.弹出如下对话框，“**Port**”选择“**Silicon Labs CP210x USB to UART Bridge(COM7)**”，单击“**Browse...**”选择之前准备好的microPython固件<span style="color: rgb(0, 209, 0);">esp32-20220618-v1.19.1.bin</span>。检查“Erase flash before installing”和“Flash mode”，然后点击“**安装**”，等待安装完成提示。（<span style="color: rgb(255, 76, 65);">注意：如果安装固件失败，请再次点击“**安装**”，然后按住ESP32主板上的Boot键![Img](./media/a3ce49fbd6f40f09869aa7e1d9f902f8.png)，出现上传进度百分比再松开Boot键。</span>）

![Img](./media/31a813b6aee6c97d1e3c1ad823afb959.png)

![Img](./media/3a22fb4f8238bacea9a880cc04461368.png)

![Img](./media/624fd845172c4f61093b03a1e8b994be.png)

4.等待安装完成。安装完成后先点击“**关闭**”再点击“**好的**”就行。

![Img](./media/f9412943c23e89b54d77943762375c74.png)

![Img](./media/ddf2a71d50fc5c5702cccc0516992c19.png)

![Img](./media/e697ce4e1d111990473cad4a56007888.png)

5.关闭所有对话框，转到主界面，点击“![Img](./media/7b5fe8311cc696a95e2436fcda1f2a41.png)”。如下图所示：

![Img](./media/7ddff7c501118105a347040e257382de.png)

6.到目前为止，一切准备工作都已就绪。

**五、测试代码：**

<span style="color: rgb(255, 218, 81);">测试Shell命令</span>

在“Shell”窗口中输入“print('hello world')”并按Enter键。

![Img](./media/a62c6c3fe3a805826b02251b5ede2233.png)

<span style="color: rgb(255, 218, 81);">在线运行</span>

ESP32需要连接到计算机时，它是在线运行。用户可以使用Thonny编写和调试程序。

1.打开Thonny并单击![Img](./media/15ef882707c025fcceb5fc78f624c946.png)“打开”。

![Img](./media/dbbcc54db4e22627a5b15c8155c46e53.png)

2.在新弹出的窗口中，单击“**此电脑**”。

![Img](./media/423687ce5fedb4a31b6b415b02d08871.png)

在新的对话框中，在路径：“<span style="color: rgb(255, 76, 65);">..\程序代码\Python_代码\项目01 Hello World</span>” 中选择 “**Project_01_HelloWorld.py**” 。

![Img](./media/d91f0f708b1a7f16a5552ca3b0934fe7.png)

![Img](./media/74b7bfdb8175388b3c34a50bcce37bad.png)

单击![Img](./media/5c05febdb56bb5ef370e897c012c1b91.png), “Hello World”将在“Shell”窗口中打印出来。

![Img](./media/b6fbe337a8053653dc74e1a567fddb8c.png)

<span style="color: rgb(255, 76, 65);">注意：</span>在线运行时，如果按下ESP32的复位键，用户的代码将不会再次执行。

六、Thonny常见的操作：

本教程中使用的代码保存在（即路径）：“**..\程序代码\Python_代码**”。

![Img](./media/c982aaf9952be57c1ab7464bc20deedb.png)

你可以把代码移到任何地方。例如，我们将代码保存在**D盘**中，<span style="color: rgb(0, 209, 0);">路径为D:\2. 项目教程</span>。

![Img](./media/f1ef150917d08d30d272d3e2d31ad5d7.png)

**上传代码到ESP32**

为了方便起见，我们以“**项目17 I2C 128×32 LCD**”为例。在“**项目17 I2C 128×32 LCD**”文件夹中选择“lcd128_32\.py”，右键单击鼠标，选择“**上传到/**”将代码上传到ESP32的根目录中。

![Img](./media/e23658670b2d06a0a88e545aa8f2eaab.png)

![Img](./media/a1e3a7adc7af65801ae0b8c9a876a476.png)

**下载代码到电脑**

在“MicroPython 设备”中选择“boot\.py”，右键选择“**下载到…**”把代码下载到你的电脑里。

![Img](./media/b2ede7ef773133633507da1bb578eef6.png)

**删除ESP32根目录下的文件**

在“MicroPython 设备”中选择“lcd128_32\.py”，右键单击它且选择“**删除**”，将“lcd128_32\.py”从ESP32的根目录中删除。

![Img](./media/3d875b62ef61c6d145c0c1d808a70164.png)

![Img](./media/7ad65c6935a821d54611e5a7b46c6ae8.png)

![Img](./media/aa5c039cec0ec453bdcec8751d7ab3c5.png)






