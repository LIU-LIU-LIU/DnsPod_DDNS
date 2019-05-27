# 利用DnsPod提供的api为家庭或者动态IP的用户制作DDNS服务(动态域名解析服务)。<br>
## For Linux<br>
## By liu.liuy@qq.com<br>

### 使用方法
### 下载文件"run",并编辑此文件，按需补充好配置，直接运行run文件即可。
### 如果提示无法执行。请赋权(chmod +x run)。

本程序发邮件功能需要用到sedEmail，请点击以下链接下载，并在/usr/local/bin下创建软连接<br>
http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz<br>
<br>
wget http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz<br>
下载sendEmail<br>
<br>
tar -zxvf sendEmail-v1.56.tar.gz<br>
解压sendEmail<br>
<br>
cd sendEmail-v1.56<br>
进入sendEmail目录<br>
<br>
ln -s sendEmail /usr/local/bin<br>
创建软连接<br>
