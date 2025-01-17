# Procedure for installing database in MSSQL Server cluster

1. In the exact path `C:\Support\en_sql_server_2019_standard_x64_dvd_c7d70add` you'll need to start the installation
2. From the installation menu selecet "cluster installation"
3. Go through the menus for the license, etc. When you get to the Instance Configuration you have to select name of installation.

   ###### EXAMPLE:

    ```
    SQL Server Network Name: BG-EXT-.....
    Named istance: "Installation name"
    ```

4. From Cluster Disk Selection choose : Cluster Virtual Disk (SQL Data)
5. From Cluster Network Configuration choose a new free for use address from the public network and attach one static form: `91.92.110.0/26`
6. In the Server Configuration menu you must select user from the Active Directory assigned to this role: `ERPNET\production\mssql.usr` and the corresponding password for it.

7. From the Database Engine Configuration menu in subcategory Server Configuration you have to select authentication mode and add the users which will be administrators of this DB. In subdirectory you'll need to check correct path for installation of DB and go through these several key points:

   [DB555_conf.ini](./procedure_hyper-v_db_installation_DB555_conf.ini)

    * You have to create directory in `C:\ClusterStorage\SQLData\InstanceName` and after that you'll need to point `INTALLSQLDATADIR="C:\ClusterStorage\SQLData\InstanceName"`
    * The max degree of parallelism (MAXDOP) server configuration option. `SQLMAXDOP="1"`
    * The number of Database Engine TempDB files. `SQLTEMPDBFILECOUNT="8"` Database Engine TempDB data file in MB. `SQLTEMPDBFILESIZE="2048"`
    * CPU affinity = 2 Cores = 4 Threads – It is set according to the license of the respective client
    * Log file growth - 64 MB by default
    * Query Store - Enabled for all DB - READ/WRITE by default

   &nbsp;
   
   From the configuration file you can make a review of all needed settings for the rest subcategories Database Engine Configuration for needs of the company, as well as the overall configuration of the new DB/instance

8. Last step shows you a summary of pre-made configuration, as well as example with the containing configuration directory and there is no issues you are able to continue forward with installation: `C:\ProgramFiles\Microsoft\SQL\Server\150\Setup\Bootstrap\Log\20221223_105439\ConfigurationFile.ini`

9. After successfull instalation you have to do testing transfers to see is it possible to do transfers between these nodes. If transfer is working from Fail Over Cluster Manager - Resources - Properties for each category of this instance (SQL server, SQL Agent and all of the rest) select that these
   two nodes to be the owner of installation.

10. If the discribed in #9 details are not working correctly it could be needed to add an instance.
    * From the second node of Windows Cluster start instalation and choose "Add Node".
    * Pick newly created (need to be detected automatically) i.e. `FAILOVERCLUSTERGROUP="SQL Server (DB555)";`
    * Also select the same address and netmask, i.e.: `FAILOVERCLUSTERIPADDRESSES="IPv4;х.х.х.х; Cluster Network 2; 255.255.255.192";`
    * And you'll need to point the correct name for network access, i.e.: `FAILOVERCLUSTERNETWORKNAME="BG1-EXT-DB555";`, and account, i.e.: `AGTSVCACCOUNT="erpnet\productionmssql.usr"; SQLSVCACCOUNT="erpnet\productionmssql.usr;`
