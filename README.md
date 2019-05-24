利用DnsPod提供的api为家庭或者动态IP的用户制作DDNS服务(动态域名解析服务)。<br>
For Linux<br>
By liu.liuy@qq.com<br>
程序需要用到SedEmail程序来提供发送邮件的功能，请先在Linux发行版中下载下方链接文件，并解压。并将sendEmail创建软链接至/usr/local/bin<br>
http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz<br>
<br>
wget http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz<br>
下载sendEmail<br>
tar -zxvf sendEmail-v1.56.tar.gz<br>
解压sendEmail<br>
cd sendEmail-v1.56<br>
切换目录<br>
ln -s sendEmail /usr/local/bin/sedemail<br>
创建软连接<br>
