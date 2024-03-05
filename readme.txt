一、更换地址：
	1.打开ac_lib,regex_lib, 将4个函数（ac-match ac-change regex-match regex-change）的keyword.txt地址路径更换成你们的主机下的地址路径。
	2.打开src目录，将main包含的头文件地址更换成你们主机下的地址路径。（若不加路径只写头文件，将导致编译失败）

二、搭建库、生成可执行文件
        
	打开终端：ctrl+alt+T
	输入：
		cd ac-regex(切换至ac-regex目录)
		cd build（切换至构建目录build）
		cmake ..(注意是空格＋两个点，建立cmake规则，构建ac_libso,regex_libso)
		make(将源文件与动态库链接，生成可执行文件main_executable)
		./main_executable(执行exe文件）
		
		即可启动该程序                     