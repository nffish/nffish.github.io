---
layout: post
title:  "Paralles Desktop 从第三方虚拟机导入"
date:   2016-09-15 21:45:00 +0800
categories: App
---
我有个Virtualbox的Ubuntu Kylin虚拟机名为UbuntuKylin.vdi的虚拟磁盘。Parallels Desktop GUI图形界面导入该虚拟磁盘的时候，发生了错误，导致转换该虚拟磁盘失败。原因是无法识别安装于磁盘上的虚拟机操作系统。  
当然这个可以通过命令行来解决。命令行下有个prl_convert工具，有一个--allow-no-os选项。  
转到UbuntuKylin.vdi文件所在目录，执行以下命令就可以将虚拟磁盘转换为Parallels Desktop的.hdd格式虚拟磁盘了。  
<code>prl_convert UbuntuKylin.vdi --allow-no-os</code>

更多有关prl_convert工具的命令可以参考[此处](http://download.parallels.com/doc/psbm/v5/rtm/Parallels_Command_Line_Reference_Guide/33718.htm)

