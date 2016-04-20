Planned downtime of Pootle
##########################

A pootle security update needs to be installed.
Due to the needed database migrations, this might take quite a long time. The update process starts on Monday, 18 April, 0300 UTC and might take up to 12 hours. During that timeframe, pootle will be offline.


Update 2016-04-20 1230UTC
=========================

The database migration is still in progress as of Wednesday, 20 April, 1230 UTC.
It is taking longer than expected by the pootle experts.

Details about the ongoing migration:

- The current database migration is the addition of a column to the largest table of pootle
- The size of the tablespace for this table alone is over 33G
- The MySQL/InnoDB database that is used uses a temporary table to store the data while a new table with the additional column is created
- The size of the temporary table is currently 9.3G
- The tablespace for the original table of 33G may contain unused space due to the structure of InnoDB
- In worst case scenario, the migration of this table alone might take until Friday

After evaluating the different options (continuing migration/aborting migration and downgrade), we decided to continue on until Friday Noon. If no sufficient progress was made by then, the migration will be aborted and the pootle installation downgraded.