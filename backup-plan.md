# Backup plan

## Office


- ### Server6

 | Backup source| Backup Destination |Schedule | Type | Retention|
|:----------|:-------------|:--------|:-----|:-----|
| ALOE-DBSvr/Vegard_ERPBG  | SYS-DPM2 / LOCALDISK O: SQLDB-01-ONLINE| Every day at 08:00 PM | Express Full Backup | 7 days|
| HQ-SYS-VPN   | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| SYS-AccessControl | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| SYS-DC2 | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| SYS-DHCPSvr | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| SYS-WiFiController | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| Sys-dc3 | - | - |- | -|
| Sys-dc5 | - | - |- | -|
| SYS-RTR-01v |  - | - |- | -|



<br>

## Data center

- ### Server12

| Backup source| Backup Destination |Schedule | Type | Retention|
|:----------|:-------------|:--------|:-----|:-----|
| BG-SYS-DC02V  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| SYS-DC6  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |

- ### Server8

| Backup source| Backup Destination |Schedule | Type | Retention|
|:----------|:-------|:--------|:---|:------|
| RemoteServer2 | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-DEV-BuildSvr | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-SUPP-SECRET  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-BETA | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-BETARDP  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-NBETA  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-NBETARDP  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-NSTABLE  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-NSTABLERDP  | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-PREV | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-PREVRDP | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days ||
| HQ-XP-STABLE | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-STABLERDP | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-TEST-WIN7 | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| HQ-XP-TEST-WIN10 | SYS-DPM2 / LOCALDISK O: VMs-ALL-01-DISK | Every day at 07:00 PM |  Express Full Backup | 7 days |
| WebSrv3 | - | - | -| -|
| SERVER4 | - | - | -| -|
| ZendeskRedirect | - | - | -| - |



- ### Server9

|Backup source| Backup Destination | Schedule | Type|  Retention| Developer|
|:----------|:-------------|:--------|:------|:----|:-------|
| DEV-WaterPVM | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM|  Express Full Backup | 7 days |  Ivo Atanasov |
| HQ-DEV-VM11 | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM|   Express Full Backup | 7 days | Kiril Rusev |
| HQ-DEV-VM12 | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM|  Express Full Backup | 7 days | Dilyan Rusev |
| HQ-DEV-VM16 | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM|  Express Full Backup | 7 days | Maria Marzovanova |
| RCT\HQ-DEV-VM41 | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM | Express Full Backup | 7 days |  Nikolay Nikolov |
| RCT\HQ-DEV-VM51 | SYS-DPM2 / LOCALDISK O: VMs-ALL-02-DISK | Every day at 06:00 PM|  Express Full Backup | 7 days | Ivan Argentinski |
|HQ-DEV-VM43 |-| -| - | - | Ognyan Ivanov |
|HQ-DEV-VM45 | - | - | - | - | Stanimir Stoykov |
|HQ-DEV-VM46 | - | - | - | - | Vasilen Stavrev |
|HQ-DEV-VM47 | - | - | - | - | Metodi Eterov |
|HQ-DEV-VM48 | - | - | - | - | Petar Kostov | 
|HQ-DEV-VM49 | - | - | - | - | Bena Yakimova |
|HQ-XP-VM21  | - | - | - | - | Ivelin Ivanov |
|HQ-XP-VM22  | - | - | - | - | Kristina Peycheva| 
|HQ-XP-VM23  | - | - | - | - | Tihomira Hristozova |
|HQ-XP-VM24  | - | - | - | - | Nadejda Traykova |
|HQ-ADM-VM18 | - | - | - | - | - |

<br>

## Cloud systems

### Cloudberry

| Plan name | Backup source | Backup destination | Schedule | Type | Skipped Folders |
|:--------|:-------|:--------|:-----|:------|:-----|
| DB50xSQL-BAK-AZURE |\\\\bg1-sys-sql5as\c$\ClusterStorage\SQLData\ | Azure Storage Account (ERP-OFFICE) | Every Monday at 3:00 AM | Incremental |   DB501 <br> DB502 <br> DB503 <br> DB504 <br> DB505 <br> DB506 <br> DB541 <br> DB553 <br> DB707 <br> DATA <br> FTData <br> JOBS <br> Log <br> repldata |
| DB50xSQL-TRN-AZURE | \\\\bg1-sys-sql5as\c$\ClusterStorage\SQLData\ | Azure Storage Account (ERP-OFFICE) | Tuesday-Friday at 3:00 AM | Incremental |  DB501 <br> DB502 <br> DB503 <br> DB504 <br> DB505 <br> DB506 <br> DB541 <br> DB553 <br> DB707 <br>  DATA <br> FTData <br> JOBS <br> Log <br> repldata |



## SQL Maintenance Plans

### Local backup
| SQL Server host | SQL Instance | Full backup| Transaction Log backup | Retention | Local backup| 
|:--------|:-------|:--------|:-----|:------|:----|
| BG1-SYS-SQL5AS  | All instances | Occurs every week on Sunday at 10:30:00 PM | Occurs every day every 60 minute(s) between 12:00:00 AM and 11:59:59 PM | 15 days | - |
| BG1-SYS-SQL5BS (cluster node) |  |  |  | |


<br>

| Database Instance | Databases List | Local Backup | CloudBackup |
|:--------|:-------|:--------|:-----|
| BG1-EXT-DB542.hosting.erp.net\DB542 | E1_EDU_TESTDB | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542 | E1_EDU_TESTDB_MODEL | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542 | E1_PLOVDIV_UNIVERSITY | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542 | E1_POPOV_HIGH_SCHOOL | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542 | E1_TECHNICAL_UNIVERSITY_SOFIA | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_TECHNICAL_UNIVERSITY_VARNA | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_UNIVERSITY_AZLATAROV_BURGAS | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_UNIVERSITY_AZLATAROV_BURGAS_TRAINING | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_UNIVERSITY_MODEL | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_UNIVERSITY_SVISHTOV | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_VTU | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_VUZF | yes | yes |
| BG1-EXT-DB542.hosting.erp.net\DB542| E1_VUZF_2020 | yes | yes |

<br>

| Database Instance | Databases List | Local Backup | CloudBackup |
|:--------|:-------|:--------|:-----|
| BG1-EXT-DB543.hosting.erp.net\DB543 | E1_ACTSOFT_DEV_BETA | yes | yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_ALGOS_SIM | Yes	| Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_APTOS_DEMO |	Yes	| Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_CRAZY_WEB_DEMO	| Yes | Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DEMODB | Yes	| Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DEMODB_MODEL	| Yes |	Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DEMOFIRM	| Yes |	Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DEV_PARTNERS_TEST |	Yes	| Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |E1_DEV_PARTNERS_TEST_BETA | Yes | Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |E1_DEV_PLAN_SOLUTIONS_DEMO | Yes |Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DEV_PLAN_SOLUTIONS_TEST |	Yes |	Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_DSK_DEMO |	Yes	|Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_EASY_M_CONSULT_TEST | Yes | Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_EDUCATION |	Yes	| Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543 |	E1_EDUCATION_TEST	| Yes |	Yes |
| BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ENTERPRISE_DEMO	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ENTERPRISE_DEMO_OLD|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ENTERPRISE_DEMO_PARTNERS|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ENTERPRISE_DEMO_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ENTERPRISE_PUBLIC|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543	|E1_ENTERPRISE_PUBLIC_BETA|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_FOURPLUS_DEMO	|Yes	|Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_FREESOFT_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_HOPIXIT_DEMO|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_IT_BUSINESS_PROJECTS_DEMO|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ITC_DEMO	|Yes	|Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ITC_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ITC_NEW_VERSIONS|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_ITC_TEST	|Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_LOGSENTINEL_TEST	|Yes	|Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_LUCKYTO_DEMO|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_METHODOLOGICAL_GUIDELINES|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_MOBILE_SELLER_DEMO|	Yes	|Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_MOBILE_SELLER_DEMO_BETA|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_MOBILE_SELLER_DEMO_PREVIOUS|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_NIMERO_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_PATHFINDER_SIM|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_PMK_CONSULT_TEST|	Yes	|Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_PUBLIC_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_DEV|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_DEV_BETA|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_MODEL_BETA|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_MODEL_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_SERVICE_DEMO| Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SBS_SERVICE_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SHARPWARE_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SIRIUS_ART_DEV|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_STARTDB|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_STARTDB_BG|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_STARTDB_BG_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_STARTDB_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_STOIC11_DEMO|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_SYNAPIO_TEST|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_TESTD|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_TESTDB_MODEL|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_UNIVERSITY_DMG|	Yes|	Yes|
|BG1-EXT-DB543.hosting.erp.net\DB543|	E1_VN_BIZU_DEMO|	Yes|	Yes|


<br>

| Database Instance | Databases List | Local Backup | CloudBackup |
|:--------|:-------|:--------|:-----|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_18_1|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_18_2|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_19_1|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_20_1|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_20211123|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_DEV_TEST|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_UPGRADER_TEST_4	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1_UPGRADER_TEST_5	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1AST_DEV	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	E1PRJ_DEV	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	IS_FIRM1	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	ISSYS	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	PC_BELLA_34	|Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	TESTS|	Yes	|Yes|
|BG1-EXT-DB551.hosting.erp.net\DB551|	TESTS2|	Yes	|Yes|

<br>

| Database Instance | Databases List | Local Backup | CloudBackup |
|:--------|:-------|:--------|:-----|
|BG1-EXT-DB554.hosting.erp.net\DB554|	confluence_enterpriseone|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	E1LIC_ALOE|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	era_db|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	ERA_ERPBG|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	FogBugz_Aloe|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	IS_ALOECO|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	ISSYS|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	SecretServer|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	STYLE_ALOE|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	Tfs_ERPBG_Configuration|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	Tfs_ERPBG_CustomerProjects|	Yes|	Yes|
|BG1-EXT-DB554.hosting.erp.net\DB554|	Tfs_ERPBG_Internal|	Yes|	Yes|

<br>

| Database Instance | Databases List | Local Backup | CloudBackup |
|:--------|:-------|:--------|:-----|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_BETA	|Yes	|Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_COMPRESS_TEST|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_CRM_ERP_EM|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_DEMOEX|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_DEMOEX_20210802|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_DEMOFIRM_DEV_TEST|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_DEMOFIRM_DEV_TEST_BETA|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_EDUCATION_OFFICE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_ERPNET_NBETA|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_MODEL_DELETE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_20190807|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_20190807_PREV|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_2020|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_20200512|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_AZURE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_DC_20211116|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NBETA_DEV_TEST|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20200609|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20200619|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20200707_BETA1|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20200715|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20200720|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20211104|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20220511|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20220511_3|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_NSTABLE_20220511_4|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_ONLINESTORE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_ONLINESTORE_2015|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_2018_2_DO_NOT_UPGRADE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20200819|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20200825|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20201029|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20201029_2|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20201120_4|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20201216|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20201216_2|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20210115|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20210419|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_PREV_20210419_2|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20210323|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20211217|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20220318_2|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20220321|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20220414|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_STABLE_20220523|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_TEST_UPGRAGE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_TESTDB_MODEL_20220413|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_UNIVERSITY|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_UNIVERSITY_TEST|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_V2016_SP28__DO_NOT_UPGRADE_OR_DELETE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_V2017_DO_NOT_UPGRADE_OR_DELETE|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	E1_V2018_SP11_DO_NOT_UPGRADE_OR_DELETE|Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	EA_DB_RESTORE_TEST|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	IS_DEMOFIRM|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	ISSYS|	Yes|	Yes|
|BG1-EXT-DB555.hosting.erp.net\DB555|	Zetta_Azure_Test2|	Yes|	Yes|
