# Installation requirements

This document summarizes the requirements, when installing, upgrading or maintaining a SQL Server for ERP.bg dev.

## 1. IFI for database files

IFI is Instant File Initialization.
IFI is required in order for DB files to grow faster.
IFI requires giving permissions to the SQL Server service account.

For more information and how to activate it, read the following:

https://learn.microsoft.com/en-us/sql/relational-databases/databases/database-instant-file-initialization?view=sql-server-ver16

SQL 2016 and later provide this option in the setup:

https://learn.microsoft.com/en-us/archive/blogs/psssql/sql-2016-it-just-runs-faster-instant-file-initialization

## 2. IFI for transaction logs

Transaction logs can also benefit from IFI.
For this to work, the auto growth increment must be setup to 64 MB.
See the link in the previous section for more information.

## 3. Lock pages in memory

Lock pakges in memory is required for optimal memory performance.
For more info and how to activate it, read the following topic:

https://learn.microsoft.com/en-us/sql/database-engine/configure-windows/enable-the-lock-pages-in-memory-option-windows?view=sql-server-ver16

To verify that LPM has activated successfully, check the SQL Server log for the following entry:
- Using locked pages in memory manager

## 4. Multiple TEMPDB files

TempDB should be created with 8 files for optimal performance.
For more information, read the following topic:

https://learn.microsoft.com/en-us/archive/blogs/psssql/sql-2016-it-just-runs-faster-automatic-tempdb-configuration

## 5. MaxDOP = 1

MaxDOP, or max degree of parallelism, should be set to 1 on the server level.
This setting is very important and is the basis for the resource management for ERP.bg.

For more information:

https://learn.microsoft.com/en-us/sql/database-engine/configure-windows/configure-the-max-degree-of-parallelism-server-configuration-option?view=sql-server-ver16

## 6. Backup plans

By default, configure the following backup plan for each SQL instance:

* Include ALL databases, including the system databases.
* Make full backup once per week, during the weekend. Make sure the timing does not overlap with index optimization jobs.
* Keep 15 days of full backups. This keeps 2 or 3 full backups. Two full backups most of the time, 3 full backups for 1 day after the last full backup.
* Make log backups every 1 hour (60 minutes).
* Keep 15 days of log files.
* Setup the maintenance jobs to clean maintenance job history.
* Do NOT use differential backups.
* Backup directly to backup server.
* Have the backup server synchronize the backups with Azure storage account at all times.

## 7. Optimization jobs

By default, setup the following optimization jobs:

* Daily - Update statistics (20% scan)
* Once per month - Index defrag
* Currently, we do not suggest having automatic "Index rebuild" at all
