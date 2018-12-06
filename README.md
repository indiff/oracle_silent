# oracle_silent
#### oracle 11g  通过自动应答文件 单机自动化安装shell脚本

## 使用方法：
	* 以root身份运行 install-oracle11g.sh
	* 以oracle身份执行下面的命令，也就是上面脚本后面注释的部分
<pre> 
su - oracle
cd /u01/oracle/database
./runInstaller -silent -force -responseFile /home/oracle/db.rsp
dbca -silent -responseFile /home/oracle/dbca.rsp
netca -silent -responsefile /u01/oracle/database/response/netca.rsp
cp oracle.init.d /etc/init.d/oracle
chkconfig oracle on
</pre>

## 默认设置：

ORACLE_SID=vnetoodb

## oracle11g 下载

[百度网盘]
(链接: https://pan.baidu.com/s/1vBcJSheEGHgRGfOtnlOFSQ 提取码: nvpn)

## TODO

不再维护



 