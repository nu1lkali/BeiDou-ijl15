# BeiDou-ijl15

将主分支的两次Release视为v1和v2。

由于v2版本在部分机器上会导致游戏进入到登录界面的时候崩溃，而v1没有这个问题，因此本分支继承主分支的v1版本，并不再和主分支同步，单独开发。

本分支主要服务于BeiDou的客户端。

## 使用方法

已测试的开发工具 VS 2019，SDK 10，工具集 VS2019（v142）

使用vs打开的时候注意，要使用 Release x86 的模式生成解决方案

生成后可在 out/Release 目录下找到 ijl15.dll

先把客户端原本的ijl15.dll重命名成2ijl15.dll，然后把生成的ijl15.dll拷贝到客户端目录下，然后把项目根目录下的config.ini同样复制到客户端目录下，具体配置都在config.ini中

## 更新记录

相比主分支 v1

- 支持中文输入/角色中文名
- 修复滚轮乱飞的问题
- 修复ToolTip超出游戏窗口的问题
- 针对中文环境的一些调整：装备tooltip字体大小，道具有效期字体大小，聊天栏的选项