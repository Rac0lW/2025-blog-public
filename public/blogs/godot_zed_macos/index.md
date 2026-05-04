**注意此为MacOS安装教程, Windows也能使用Zed作为外部编辑器, 但是需要安装ncat, 但是会有Bug(目前尚未解决)**

首先安装好Zed Editor以及Godot 4.0以上版本

Zed Editor地址: https://zed.dev/download

然后在Godot中打开Editor Settings

在Text Editor的External栏目中

在Exec Path中直接输入 *zed* 或者 你的Zed.App的安装地址

在Exec Flag中输入{project} {file}:{line}:{col} 

在Use External Editor中 开启就行



