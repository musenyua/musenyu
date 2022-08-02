`yum -y install lm_sensors ipmitool -y`

`ipmitool lan print 1`

`ipmitool -I lanplus -H 192.168.0.120 -U root -P calvin raw 0x30 0x30 0x01 0x00`

`ipmitool -I lanplus -H 192.168.0.120 -U root -P calvin raw 0x30 0x30 0x02 0xff 0x1e`

`ipmitool sensor|grep Fan`

最后的0x0a表示转速的百分比的十六进制，0a表示10%，0f表示15%。1e表示30，28表示40%；32表示50%

（如果命令不发执行，去idarc里面配置-网络，启用lan上的IPMI）

