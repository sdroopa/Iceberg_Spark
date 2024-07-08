# Iceberg_Spark
The objective of this git hub project is to prepare the examples demonstrating the features of Iceberg Tables using the Jupyter notebook with spylon kernel and scala programming language with below configurations.
Iceberg version 1.5.2
Spark Version 3.5.1
Jupyter notebook with Spylon Kernel



- [Introduction](#introduction)
- [Iceberg Features](#outlook-account)
  * [Schema Evolution](#add-update-delete-changetype)    

 
## Introduction
Iceberg is an open source table format to perform huge analytics with high - performance. Iceberg is designed to manage large analytics table with either of the supported multiple formats like Parquet, Avro and Orc. 
This is often compared with Delta lake format. Delta lake format is integrated with Databricks platform while Iceberg is interoperable and can work with different  engines like Spark, Trino, Flink, Presto, Hive and Impala. Apache Iceberg is supported with partition evolution alongside schema evolution.
 

## Iceberg Features


### Schema Evolution[1] 
source : https://iceberg.apache.org/docs/1.5.2/evolution/#schema-evolution
Iceberg supports the following schema evolution changes:

Add -- add a new column to the table or to a nested struct
Drop -- remove an existing column from the table or a nested struct
Rename -- rename an existing column or field in a nested struct
Update -- widen the type of a column, struct field, map key, map value, or list element
Reorder -- change the order of columns or fields in a nested struct
Iceberg schema updates are metadata changes, so no data files need to be rewritten to perform the update.

####Iceberg_SchemaEvolution.ipynb 
This notebook is aimed at running schema evolution cases by adding new column, updating and deleting columns of different datatype.



