#服务器优化工具

```
https://raw.githubusercontent.com/cnmars/serverscript/main/tool.sh
```

#使用方法


```
/etc/sysctl.conf
```

```
     net.ipv4.ip_forward=1
     net.ipv4.tcp_congestion_control=bbr
     net.core.default_qdisc=fq
     net.core.rmem_max = 67108864
     net.core.wmem_max = 67108864
     net.ipv4.tcp_rmem = 4096 87380 67108864
     net.ipv4.tcp_wmem = 4096 65536 67108864
     net.ipv4.tcp_congestion_control=bbr
     net.ipv4.tcp_mtu_probing=1
     net.core.default_qdisc = fq
     net.ipv4.tcp_thin_linear_timeouts=1
     net.ipv4.tcp_fastopen=3
```
保存生效
```
sysctl -p && reboot
```
