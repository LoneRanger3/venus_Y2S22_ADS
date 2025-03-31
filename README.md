# venus_Y2S22_ADS
sa100 yizhi

编译：
1，编译报错时先clean一下；
$ ./build.sh clean

2，编译配置。
$ ./build.sh config
都选0（fastboot也选0，关闭）。

3，编译打包。
$ sudo ./build.sh

Entry Point:  00000000
pack finish!
pack finish!
pack venus_n7v1_cdr_2025-03-31.pkg ok

固件路径：
W:\xdsm\yizhi\keshi\sa100\git_sa100\venus_Y2S22_ADS\pack\platform\n7\v1\cdr

4，卡升级bin文件制作。
C:\Users\A\Desktop\pkg2rom
4.1，替换pkg2rom下的pkg文件，pkg2rom.bat中的也替换。
venus_n7v3_sar_rel_2022-04-20.pkg
4.2，执行pkg2rom.bat。
4.3，out下生成卡升级bin文件。

把bin文件拷贝到sd卡，重新上电自动升级。