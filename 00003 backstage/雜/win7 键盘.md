那么在一台使用日文键盘的PC上安装了中文版Windows 7后，该如何设置键盘布局呢？

Windows 7的安装界面有一个很容易让人疑惑的选项。在第一个界面，安装程序就可以让你选择“键盘和输入方法”。
点击那个下拉菜单，可以找到“日语”的选项。也许有人和我一样，当时以为在这里选了日语之后问题就搞定了。
可惜安装完毕之后他们也会和我一样失望的发现问题依然。按下键盘上的“@”键，出现的却是“[”字符。

此时，到“控制面板”->“区域和语言”->“更改键盘…”的“常规”页面，可以看到“中文（简体，中国）”的子项目中
确实被预设了“日语”。

那为什么键盘的布局和按键实际显示的字符还是不符呢？其实Windows安装程序在初始时确实询问了用户希望使用的键盘布局，但这充其量是帮助用户设定初始化的ASCII字符输入状态时的布局而已。而且也仅仅是做了一半工作，要正确显示和键盘布局相符的字符，我们还需要正确的键盘驱动程序。用一句话来总结，Windows 7输入法程序做好了使用日语键盘的准备工作，但是键盘驱动程序却还没准备好。这一点，正如我几年前写的简介一样，微软依然没有做到自动甚或只是半自动识别而已。

不过留给我们的工作也很简单，只是修改一下键盘的驱动程序而已。不过这次可不是在控制面板的“键盘”中进行的。取而代之，我们必须进入“设备管理器”，找到“键盘”分类。由于时代的进步，现在已经很少有人还在继续使用PS2接口的键盘，USB键盘已经毫无疑问成为了主流。

双击“键盘”下的“HID Keyboard Device”，在“驱动程序”页点击“更新驱动程序…”。然后依次点击“浏览计算机以查找驱动程序软件”->“从计算机的设备驱动程序列表中选择”，并去掉“显示兼容硬件”前的勾。

此时你应该能看到列表分成了左右两列。在左侧的“厂商”列表中选择“Toshiba”，然后选择右侧列表中的“Toshiba USB 109 Japanese keyboard”。最后点击下一步，并无视Windows无法验证驱动程序与硬件兼容性的警告，直接按“是”进行安装。

如果你的键盘依然是PS2接口的话，那么在厂商列表可以选择“(标准键盘)”，并选择右侧列表中的“Japanese PS/2 Keyboard (106/109 Key)”。

安装完驱动程序后打开写字板验证一下吧，上面的修改应该已经起作用了。

最后补充一条，当你处于中文输入状态时，你的键盘依然是处于标准英语布局。只有从中文输入状态按下Shift+Ctrl切换到ASCII输入状态时，你的键盘布局才会变成日语模式

