## Office

- ### Server6

|  VM name | Purpose | OS | IP address |
|---|:---|:---:|:---|
| ALOE-DBSvr  |  SQL 2014 - use only for Access control| Windows Server 2008 Enterprise    | 192.168.0.13 |
| SYS-AccessControl  |  Software for Access control | Windows Server 2012 Standard   | 192.168.0.74   | 
| HQ-SYS-VPN |  RA VPN SSTP  - use only for office networks| Windows Server 2012 R2 Standard | 192.168.0.18 |
| Sys-dc2 | Certification Authority, IIS| Windows Server 2012 Standard | 192.168.0.18 |
| Sys-dc3 | Domain Controller, DNS for aloeco.com| Windows Server 2012 R2 Standard | 192.168.0.26/ 192.168.41.168 |
| Sys-dc5 | Domain Controller for aloeco.com| Windows Server 2012 R2 Standard | 192.168.0.200 |
| sys-router2 | DHCP, IIS | Windows Server 2012 R2 Standard | 192.168.0.50 |
| SYS-RTR-01v | PfSense FW | FreeBSD | 192.168.0.18 |
| SYS-WiFiController | WiFi Controller | Ubuntu 14.04 LTS | 192.168.42.186 |

&nbsp;

## Data Center

- ### Server8

|  VM name | Purpose | OS | IP address  |
|---|:---|:---:|:---|
| RemoteServer2 | Default Windows apps + E1 instance for internal purposes| Windows Server 2012 Standard | 192.168.8.57 |
| WebSrv3 | Fogbugz - internal ticket system| Windows Web Server 2008 R2 | 91.92.110.24 |
| HQ-DEV-BuildSvr | Default Windows apps + E1 build server | Windows Server 2016 Standard | 192.168.8.77 |
| SERVER4 | Default Windows apps (File Server) | Windows Server 2019 Standard | 192.168.8.50 |
| HQ-SUPP-SECRET | Thycotic secret server - internal system for credentials |Windows Server 2012 R2 Standard | 192.168.8.58 |
| HQ-XP-BETA | Default Windows apps + E1 dev environment | Windows server 2016 Standard | 192.168.8.75 |
| HQ-XP-BETARDP  | Default Windows apps + E1 dev environment | Windows server 2016 Datacenter | 192.168.8.76 |
| HQ-XP-NBETA | Default Windows apps + E1 dev environment | Windows server 2016 Standard | 192.168.8.73 |
| HQ-XP-NBETARDP | Default Windows apps + E1 dev environment | Windows server 2016 Datacenter | 192.168.8.60 |
| HQ-XP-NSTABLE | Default Windows apps + E1 dev environment |  Windows server 2016 Standard | 192.168.8.73 |
| HQ-XP-NSTABLERDP | Default Windows apps + E1 dev environment | Windows server 2016 Datacenter | 192.168.8.53 |
| HQ-XP-PREV | Default Windows apps + E1 dev environment | Windows server 2016 Standard | 192.168.8.51 |
| HQ-XP-PREVRDP | Default Windows apps + E1 dev environment | Windows server 2016 Datacenter | 192.168.8.61 |
| HQ-XP-STABLE | Default Windows apps + E1 dev environment | Windows server 2016 Standard | 192.168.8.55 |
| HQ-XP-STABLERDP | Default Windows apps + E1 dev environment | Windows server 2016 Datacenter | 192.168.8.52 |
| HQ-XP-TEST-WIN7| for tests | Windows 7 | 192.168.8.61 |
| HQ-XP-TEST-WIN10| for tests | Windows 10 | 192.168.8.66 |
| HQ-XP-TEST-WIN11| for tests | Windows 11 | 192.168.8.195 |
| HQ-XP-TEST-WINSER22| for tests | Windows Server 2022 | 192.168.8.193 |
| ZendeskRedirect | support.erp.bg->support.erp.net| Ubuntu 20.4 | 192.168.8.221 |

&nbsp;

- ### Server9

|  VM name | Purpose | OS | IP address  |
|---|:---|:---|:---|
| DEV-WaterPVM | Developer Desktop Ivo Atanasov | Windows 10 | 192.168.8.64 | 
| HQ-ADM-VM18 | Developer Desktop | Windows 10 | 192.168.8.135 |
| HQ-DEV-VM11 | Developer Desktop Kiril Rusev | Windows 10 | 192.168.8.54 |
| HQ-DEV-VM12 | Developer Desktop Dilyan Rusev | Windows 10 | 192.168.8.71 |
| HQ-DEV-VM16 | Developer Desktop Maria Marzovanova | Windows 10 | 192.168.8.56 | 
| HQ-DEV-VM41 | Developer Desktop Nikolay Nikolov | Windows 10 | 192.168.8.65 | 
| HQ-DEV-VM43 | Developer Desktop Ognyan Ivanov | Windows 10 | 192.168.8.129 |
| HQ-DEV-VM45 | Developer Desktop Stanimir Stoykov | Windows 10 | 192.168.8.130 |
| HQ-DEV-VM46 | Developer Desktop Vasilen Stavrev | Windows 10 | 192.168.8.131 |
| HQ-DEV-VM47 | Developer Desktop Metodi Eterov | Windows 10 | 192.168.8.132 | 
| HQ-DEV-VM48 | Developer Desktop Petar Kostov | Windows 10 | 192.168.8.133 |
| HQ-DEV-VM49 | Developer Desktop Bena Yakimova | Windows 10 | 192.168.8.134 |
| HQ-DEV-VM51 | Developer Desktop Ivan Argentinski | Windows 10 | 192.168.8.67 | 
| HQ-XP-VM21 | Developer Desktop Ivelin Ivanov | Windows 10 | 192.168.8.68 |
| HQ-XP-VM22 | Developer Desktop Kristina Peycheva | Windows 10 | 192.168.8.70 | 
| HQ-XP-VM23 | Developer Desktop Tihomira Hristozova | Windows 10 | 192.168.8.63 |
| HQ-XP-VM24 | Developer Desktop Nadegda Traykova | Windows 10 | 92.168.8.127 | 

&nbsp;

- ### Server12

|  VM name | Purpose | OS | IP address  |
|---|:---|:---|:---|
| BG-SYS-DC02V | Domain controller - hosting.erp.net (Zetta) | - | 91.92.110.86| 
| SYS-DC6 | Domain controller, DHCP, DNS - aloeco.com | Windows Server 2012 R2 Standard | 192.168.8.42 |
| SYS-DPM2 | Backups | Windows server 2016 Standard | 192.168.8.91 / 91.92.110.100 

&nbsp;

- ### BG1-SYS-HPV02S (Zetta)

|  VM name | Software/Role  | OS   | IP address  |
|---|:---:|:---:|:---:|
| DEV-TFSSvr | TFS - for build, scripts for DB | Windows Server 2012 R2 Standard |91.92.110.94
| BG1-SYS-RAS02V | RA VPN to DC | Windows server 2016 Standard | 91.92.110.227/ 192.168.8.90
