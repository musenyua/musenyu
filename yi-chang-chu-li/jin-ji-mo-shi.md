1. 输入密码，进入紧急模式
2. `mount -o remount,rw /`
3.   把系统盘的两个挂载点以外的挂载点都\#注释掉，保存退出
   ```
   vim /etc/fstab
   ```
4. 重启设备
   ```
   reboot
   ```



