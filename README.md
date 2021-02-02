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

### Help
tleite@bsd.com.br
