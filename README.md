# zabbix-windows-disk-performance

This template discover physical disks through a powershell script.

It is based on two other templates:
<https://share.zabbix.com/operating-systems/windows/windows-physical-drive-iops>
<https://share.zabbix.com/operating-systems/windows/windows-disk-performance>

Installation process:

* Import the template to Zabbix Server.

* Put the script 'discoverdisks.ps1' in your scripts path, e.g. `C:\Program Files\zabbix_agent\scripts`. Please keep in mind that you need to adjust path in template before import or in Zabbix after import.

* Add following parametrs into Zabbix Agent config file:

```bash
Timeout=10
EnableRemoteCommands=1
UnsafeUserParameters=1
```

It has been tested with Zabbix 4.0
