# 利用DnsPod提供的api为家庭或者动态IP的用户制作DDNS服务(动态域名解析服务)。<br>
## For Linux<br>
## By liu.liuy@qq.com<br>

### 支持的功能:<br>
1检测当前域名是否和本机外网IP解析条目相同，否则邮件通知用户自行更改。(通用)<br>
2自动检测域名解析，更改为本机外网IP，并邮寄通知。(仅限Dns_Pod和腾讯云)<br>
当邮件发送一次后，就不会再发送了，必须等到下次检测到域名解析和外网IP相同时才会再次刷新。如果需要再次提醒请删除运行目录下的Express.txt文件，<br>
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
ln -s `pwd`/sendEmail /usr/local/bin/sendemail<br>
创建软连接<br>
