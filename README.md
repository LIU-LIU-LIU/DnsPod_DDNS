利用DnsPod提供的api为家庭或者动态IP的用户制作DDNS服务(动态域名解析服务)。
For Linux
By liu.liuy@qq.com
程序需要用到SedEmail程序来提供发送邮件的功能，请先在Linux发行版中下载下方链接文件，并解压。并将sendEmail创建软链接至/usr/local/bin
http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz

wget http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz
下载sendEmail
tar -zxvf sendEmail-v1.56.tar.gz
解压sendEmail
cd sendEmail-v1.56
切换目录
ln -s sendEmail /usr/local/bin/sedemail
创建软连接
