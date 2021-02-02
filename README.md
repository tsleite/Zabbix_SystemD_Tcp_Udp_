# Monitoring with Zabbix

* Services - SystemD
* Protocol - Tcp
* Protocol - Udp
* Login Attempt
* Who is logged in


## How to

1) Import template <Template_Discovery_TUProcSystemD.xml>;
2) Import file <discovery_TUProcSystemD.conf> on the directory "/etc/zabbix/zabbix_agentd.d"
3) Restart daemon or process zabbix agent;

```
Option - Alter Macro Zabbix User
{$UPDATE.DISCOVERY} - 6h
{$UPDATE.ITEM} - 2m
```

### Images

1) Template
![discovery_template](https://github.com/tsleite/Zabbix_SystemD_Tcp_Udp_/blob/main/Discovery_template.png?raw=true)

2) Test Problem - Login Attempt
![problem_login_attempt](https://github.com/tsleite/Zabbix_SystemD_Tcp_Udp_/blob/main/problem01_login_attempt.png?raw=true)

3) Test Problem - Service ( systemD )
![problem_systemd_services](https://github.com/tsleite/Zabbix_SystemD_Tcp_Udp_/blob/main/problem02_service_systemd_elasticsearch.png?raw=true)


#### Help
tleite@bsd.com.br
