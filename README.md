# back-up-and-recovery-for-database
This repository is all about how to take back ups and recover databases.

## Back up and recovery
Back ups are essential part of any IT operations, be it database back up, file system back up, server back up, etc. In case of any failure or unexpected situation like data corruption, the database system can recover to the previous state from back up.

## Methods to take back up and recover in **Postgresql**

There are three different approaches to backing up Postgresql data according to official documentation. [Postgresql Docs on Back up and recovery](https://www.postgresql.org/docs/current/backup.html).

1. SQL Dummp
2. File system level backup
3. Continuous archiving
