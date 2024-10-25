# Some useful DB2 SQL Scripts

## setmaintenance.sh and automaint.sql

Scripts should be started as instance owner! When you call setmaintenance.sh the script:

 * generates a list of databases in the instance
 * calls automaint.sql for each database
    * activates Online- and Offline Timeframes
    * set parameters for Reorg, Backup and so on

 * YOU SHOULD: change the path of your BACKUP Directory in Line 4 of automaint.sql