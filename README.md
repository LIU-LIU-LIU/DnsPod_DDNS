# 利用DnsPod提供的api为家庭或者动态IP的用户制作DDNS服务(动态域名解析服务)。<br>
## For Linux<br>
## By liu.liuy@qq.com<br>

### 支持的功能:<br>
采用了多种获取外网的接口，如果一种失败会自动重试下一种方案，并判断获取IP是否规范。   
1检测指定域名是否和本机外网IP解析条目相同，否则邮件通知用户自行更改。(通用)<br>
2自动检测域名解析，更改为本机外网IP，并邮寄通知。(仅限Dns_Pod和腾讯云)<br>
> 当邮件发送一次后，就不会再发送了，必须等到下次检测到域名解析和外网IP相同时或者距离上次发送邮件时隔7天才会再次发送邮件。<br>
> 如果需要再次提醒请删除运行目录下的Express.txt文件，<br>
> 当程序检测到外网IP和域名解析结果相同时或者上次发送邮件距现超过7天时会自动删除Express.txt文件，以便下一次通知邮件。
## 使用方法
### 下载文件"get_ip和run",并编辑"run"文件，按需补充好配置，直接运行run文件即可。
### 如果提示无法执行。请赋权(chmod +x)。

本程序发邮件功能需要用到sedEmail，请点击以下链接下载，并在/usr/local/bin下创建软连接<br>
http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz<br>
<br>
```shell
#wget http://caspian.dotconf.net/menu/Software/SendEmail/sendEmail-v1.56.tar.gz
\\下载sendEmail

#tar -zxvf sendEmail-v1.56.tar.gz
\\解压sendEmail

#cd sendEmail-v1.56
\\进入sendEmail目录

#ln -s `pwd`/sendEmail /usr/local/bin/sendemail
\\创建软连接
```
--- 
> 2021年1月29日更新:添加aliyun_dns支持
# aliyun_DDNS
# 使用aliyun_cli工具为非固定IP写的DDNS(动态域名解析服务)脚本<br>
> 如果需要发送邮件，也同样需要上述的方法配置sendeamil工具。
## 使用方法:
### aliyun_cli
1. 下载cli,前往[aliyun](https://help.aliyun.com/document_detail/121541.html)下载阿里云CLI,并按照官方文档配置好环境变量。
2. 按照[aliyun_cli配置凭据](https://help.aliyun.com/document_detail/121258.html)文档配置凭据无误后alyun命令行工具就算配置完成。
### 下载文件"get_ip和aliyun_run",并编辑"aliyun_run"文件，按需补充好配置，直接运行aliyun_run文件即可。
### 如果提示无法执行。请赋权(chmod +x)。
