[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2023-DA260)](https://api.reuse.software/info/github.com/SAP-samples/teched2023-DA260)

# DA260 - New Approaches to Loading, Staging, and Integrating Data in SAP Datasphere

## Description

This hands-on workshop will give you the opportunity to use the new replication and transformation features of SAP Datasphere. Find out how the SAP Datasphere solution helps the line-of-business user to get the job done. Discover flexible connection features. Learn how you can access data from sources. Try out the new transformation flow feature, to stage data. 

SAP Datasphere, the evolution of SAP Data Warehouse Cloud and SAP Data Intelligence, is a comprehensive data service acting as a business data fabric that enables every data professional to deliver seamless and scalable access to mission-critical business data. SAP Datasphere enables access to authoritative data by accelerating time-to-value by automatically reusing the semantical definitions and associations from SAP applications. SAP Datasphere enriches all data projects by harmonizing heterogeneous data into a business semantic model of your diverse data landscape. On top it helps to simplify the data landscape and accesses all your data across hybrid and cloud environments no matter where it resides.

## Overview

MyCompany sales bikes to customers. In the source the list price is stored in the product master data. The sales order items only contain the net sales and quantity. The list price, that was valid at the time of sales, is not stored. The goal of the exercise is, to create a data model that stores the historic list price. For that a two stage data model is used. The data will come in by a Replication Flow and be taged by a Transformation Flow. 

Question to answer: Was there a rebate in the net sales compared to the list price of the product master data?

* Learning Goal: Learn how to load data in delta with a replication flow and stage them with transformation flow.* 
* Time: 2-4 h
* Finished Product: A view that shows the potential rebate per sales order line item. 

## Requirements

* Google Chrome
* Access to this GitHub repository
* [Access to a SAP Datasphere tenant](https://academy.ap11.hcs.cloud.sap/dwaas-ui/index.html)
* Tenant access password: ObqJ7HK7gh1!
* Basic knowhow about the usage and integration of data from SAP S/4HANA
* General understanding of Enterprise Data Management and ETL (Extraction, Transformation, Load)

## Deep Dives

- [Deep Dive 0 - Introduction to the Enterprise Procurement Model (EPM) in SAP S/4HANA](exercises/dd0/)
- [Deep Dive 1 - ABAP CDS View based data extraction from SAP S/4HANA on-premise](exercises/dd1/)
- [Deep Dive 2 - Introduction to Replication Flows in SAP Datasphere](exercises/dd2/)

## Exercises

- [Exercise 1 - Replicate CDS Views from SAP S/4HANA via Replication Flows to SAP Datasphere](exercises/ex1/)
- [Exercise 2 - Transforming data using Transformation Flows in SAP Datasphere](exercises/ex2/)
- [Exercise 3 - Preparing Analytical Dataset with historic and delta records.](exercises/ex3/)
    - [Exercise 3.1 - Create an Analytical Dataset model with transformation flow generated target delta table](exercises/ex3#exercise-31---create-an-analytical-dataset-model-with-transformation-flow-generated-target-delta-table)
    - [Exercise 3.2 – Update source table record in Data Maintenance editor](exercises/ex3#exercise-32--update-source-table-record-in-data-maintenance-editor)
    - [Exercise 3.3 – Execute Transformation flow to pull the delta records from source](exercises/ex3#exercise-33--execute-transformation-flow-to-pull-the-delta-records-from-source)
    - [Exercise 3.4 – Preview the Analytical dataset model to see the historical and latest pulled records from Transformation flow Delta local table](exercises/ex3#exercise-34--preview-the-analytical-dataset-model-to-see-the-historical-and-latest-pulled-records-from-transformation-flow-delta-local-table)
- [Exercise 4 - Replicate data from SAP S/4HANA to SAP HANA Data Lake Files using Replication Flows](exercises/ex4/) 

  
**IMPORTANT**

Your repo must contain the .reuse and LICENSES folder and the License section below. DO NOT REMOVE the section or folders/files. Also, remove all unused template assets(images, folders, etc) from the exercises folder. 

## Contributing
Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) to understand the contribution guidelines.

## Code of Conduct
Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
