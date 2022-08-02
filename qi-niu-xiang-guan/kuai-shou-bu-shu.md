### **快手部署**

1. #### 首先进行拨号
2. #### 更改hostname名字

   #### 

   > 根据yg-地区-客户简称-ct/cm/cu-台数规格命名ct电信，cu联通，cm移动
   >
   > 例如重庆左总上了一台电信，就可以命名为yg-chongqing-zuozong-ct01,最后面的编号查一下用户有几台设备了，就怎么命令

   `hostnamectl set-hostname yg-chongqing-zuozong-ct01`

3. #### 执行格式化硬盘操作

   ```
   curl -o /usr/bin/yg_diskinit.sh http://hnyunbi.com/download/script/yg_diskinit.sh && chmod 777 /usr/bin/yg_diskinit.sh && yg_diskinit.sh
   ```
4. #### 执行快手部署任务

   ```
   curl -o /usr/bin/yg_ksstart.sh http://hnyunbi.com/download/script/yg_ksstart.sh && chmod 777 /usr/bin/yg_ksstart.sh && yg_ksstart.sh
   ```
5. #### 任务检查

   ```
   curl https://pcdn-quality-log.qnqcdn.net/ksp2p/ksp2p_service_check.sh -s | bash
   ```



