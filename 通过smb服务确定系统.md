# 通过smb服务确定系统
* search smb_version扫描模块
* use auxiliary/scanner/smb/smb_version 调用模块
* show options 查看选项 
* 设置选项 
    * set THREADS 10
    * set RHOSTS 192.168.1.109
* run 运行 
    * 192.168.1.101:445 is running Windows 8.1 Pro (build:9600) (name:PC-201501180647) (domain:WorkGroup)
    * [*] Scanned 1 of 1 hosts (100% complete)
    * [*] Auxiliary module execution completed
