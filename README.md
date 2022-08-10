# pycTopy
一个基于uncompyle6的批量反编译pyc脚本
由于uncompyle6对批量反编译的支持不太友好,常常需要我们自己去挨个执行命令，该工具可以在保留源来项目结构下将目标项目中的所有pyc文件还原为py代码
运行前请确保安装了uncompyle6并且python版本能支撑uncompyle6的正常运行(目前最高支持只到3.8),如果你的机器上py版本高于3.8请安装低版本python
uncompyle6安装命令:
pip/pip3 install uncompyle6

pycTopy使用命令
pycTopy targetpath
该程序会将targetpath下(包括子目录)的所有pyc文件还原为py文件，执行结束后原有的pyc文件会被删除,如果某个pyc文件反编译出错了则会保留改pyc文件并输出错误提示
