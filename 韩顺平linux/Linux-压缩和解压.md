## 压缩和解压

### gzip指令

语法：gzip 文件

描述：压缩文件，只能将文件压缩为*.gz文件



### gunzip指令

语法：gunzip 文件.gz

描述：解压缩文件命令



### zip指令

语法：zip 【选项】 xxx.zip 将要压缩的内容

常用选项：

-r：递归压缩，即压缩目录

描述：用于压缩文件和目录



### unzip指令

语法：unzip 【选项】xxx.zip

常用选项：

-d<目录>：指定解压后文件的存放目录

描述：用于解压文件



### tar指令

语法：tar 【选项】xxx.tar.gz 打包的内容

选项：

-c：产生.tar打包文件

-C：切换到指定目录

-v：显示详细信息

-f：指定压缩后的文件名

-z：打包同时压缩

-x：解包.tar文件

描述：

打包指令，最后打包后的文件是.tar.gz的文件

例如：

tar -zcvf xxx.tar.gz 文件	//压缩文件

tar -zxvf xxx.tar.gz			//解压文件

tar -zxvf xxx.tar.gz -C 指定目录			//解压文件并放在指定目录

