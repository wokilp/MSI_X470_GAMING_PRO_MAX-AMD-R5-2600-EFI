# MSI_X470_GAMING_PRO_MAX-AMD-R5-2600-EFI
黑苹果EFI
支持MAC OS BIG SUR和10.15
配置列表：
CPU：AMD-R5-2600
主板：MSI_X470_GAMING_PRO_MAX
内存：科赋DDR4 2666 16G（8*2）
显卡：蓝宝石RX470超白金
硬盘：铠侠RC10 500G
引导工具：opencore 0.6.3（20201104已更新）
注意：安装使用前要自己配三码，请使用OpenCore Configurator配置SystemSerialNumber、MLB以及SystemUUID，否则有概率会无法登陆APPLE ID
注意：理论上主板型号一致，AMD锐龙1代，2代，3代（amd早期打桩机、推土机等型号不支持，只支持锐龙1、2、3代不带核显型号）不带核显型号和RX470、RX480、RX570、RX580显卡可以通用这个efi，硬盘（三星pm981例外）和内存型号和频率也不影响。
默认不支持win10双系统启动，安装win10和big sur双系统需要使用ProperTree工具在config.plist配置文件中Misc-BlessOverride下新增子项，并添加win10引导（\EFI\Microsoft\Boot\bootmgfw.efi），并且需要修改Misc-Boot-ShowPicker的布尔值为true.
双硬盘win10和big sur双系统，需要把bigsur所在硬盘在BIOS里设置为第一引导项
单硬盘win10和big sur双i系统 ，需要参考此教程：http://imacos.top/2020/04/06/1559/
