# DNAnother

## 欢迎

这是 DNAnother 的说明文档，它将以向导的身份来指导您使用 DNAnother 的每一个功能。  
以下是文档目录：  
1 [初级功能](#初级功能)  
1.1 [创建一个项目](#创建一个项目)  
1.2 [解压分区](#解压分区)  
1.3 [安装插件](#安装插件)  
1.4 [重新打包](#重新打包)  
2 [高级功能](#高级功能)  
2.1 [高级转换](#高级转换)  
2.2 [调整额外参数](#调整额外参数)  
3 [面向开发者](#面向开发者)  
3.1 [创建插件](#创建插件)  
3.2 [为项目做点贡献](#为项目做点贡献)

# 初级功能

## 创建一个项目

您需要新建一个空文件夹才能开始项目。  
首先，您需要在命令行中打开程序。在弹出的窗口中选择您创建的文件夹，才能开始下一步操作。  
选择完后，您需要选择一个 ROM（zip 文件），将会为您自动解压。  
不选择的情况下也可以继续，但大部分功能不可用。

## 解压分区

在主画面选择「解压」，勾选您需要解压的分区，点击确定后静待过程完成。  
解压完成的分区会被放在项目下的 target 文件夹。  
您可以在其他->清空 target 来清空这个文件夹。

## 安装插件

在主画面选择「安装」，然后找到插件（zip 文件），确定后静待就安装完成了。  
用时取决于第三方脚本效率，电脑配置，插件大小等因素。

## 重新打包

在主画面选择「打包」，会指引您完成 ROM 打包向导。  
整个过程可能用时 5 分钟或更长，取决于 ROM 的大小。

# 高级功能

## 高级转换

您可以选择其他->高级转换来使用高级转换功能。  
输入 **原格式->目标格式** 这样的内容来为程序指定路线，将会为您智能解包/打包。可以在项目的 conv 文件夹查看结果。  
由于有可能会坏 ROM 所以请少用。

## 调整额外参数

通过点选其他->调整额外参数来调整**zip**和**brotli**的参数。  
一般情况下，不动它们可以获得较好的压缩品质和较快的速度(警告:乱改参数可能导致**无法打包**。)

# 面向开发者

## 创建插件

首先，根目录必须要**有一个 [install.sh](#创建插件)**。在安装插件时会直接执行这个 sh 文件。  
您将会被导航到 target 文件夹。如果需要从 base 文件夹复制内容，请使用../base/(文件)。这是完全安全的。  
如果您想要访问分区，则它们位于./(分区名字)。  
祝您写得开心！虽然我没有注重这个功能。:p  
其余的?请自由发挥:)

## 为项目做点贡献

您可以更改代码，然后提交一个 pull request。开发者在核实您的代码无恶意后会 merge。  
请不要想着捐赠。我只是一个用轮子造车的。有那点钱买点零食吃，或者给交 pr 的开发者和造轮子的大佬，都是可以的。