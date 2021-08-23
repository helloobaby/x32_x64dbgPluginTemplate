sdk和exe为snapshot_2021-07-01_23-17。

镜像下载地址https://sourceforge.net/projects/x64dbg/files/snapshots/

本仓库旨在更简单的编写x32/x64dbg插件。原作者的仓库只能一键弄出x64dbg的插件模板，

而且如果要改成x32dbg的话对不会用CMake的人来说有点困难。

步骤：

1.将x64dbg文件夹内的pluginsdk和release全部复制到本项目目录下(保证有目录\pluginsdk和\release)，因为所有路径都为相对路径

2.插件生成路径$(SolutionDir)Release\x32\plugins\PlugTest.dp32 

右键属性，链接器->常规->输出文件可以改生成的DLL(.dp32)名字，默认为PlugTest

3.x64的插件配置同上

4.只配置了Debug版本的，如果Release的话需要把Debug的配置复制一下就行了