## Step by step instruction for the creation of hybrid partitioned tables

This folder provides step by step instruction to create a hybrid partitioned table. the example uses table EMPLOYEES from schema HR.  

- 1-create-partitioned-table.sql: create a partitioned table and add rows

- 2-add-external-attribute.sql: Use ALTER TABLE command to add external partition attribute 

- 3-create-external-data.sql: Create external helper table with ORACLE_DATAPUMP

- 4-add-external-partition-data.sql: Use EXCHANGE PARTITION to provide data for the external partition

- monitor-external-part-tables.sql: Use ALL_EXTERNAL_TAB_PARTITIONS

- monitor-hybrid-tables.sql. Use ALL_TABLES with column hybrid
