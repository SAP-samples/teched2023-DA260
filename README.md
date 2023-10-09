[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2023-DA260)](https://api.reuse.software/info/github.com/SAP-samples/teched2023-DA260)

# DA260 - New Approaches to Loading, Staging, and Integrating Data in SAP Datasphere

## Description

This hands-on workshop will give you the opportunity to use the new replicatipon and transformation features of SAP Data Warehouse Cloud. Find out how the SAP Data Warehouse Cloud solution helps the line-of-business user to get the job done. Discover flexible connection features. Learn how you can access data from sources. Try out the new transformation flow feature, to stage data. 

## Overview

MyCompany sales bikes to customers. In the source the list price is stored in the product master data. The sales order items only contain the net sales and quantity. The list price, that was valid at the time of sales, is not stored. The goal of the exercise is, to create a data model that stores the historic list price. For that a two stage data model is used. The data will come in by a Replication Flow and be taged by a Transformation Flow. 

Question to answer: Was there a rebate in the net sales compared to the list price of the product master data?

* Learning Goal: Learn how to load data in delta with a replication flow and stage them with transformation flow.* 
* Time: 2-4 h
* Finished Product: A view that shows the potential rebate per sales order line item. 

## Requirements

* Google Chrome
* Access to this GitHub repository
* Access to a Guided Experience system of SAP Data Warehouse Cloud tenant (if you don't have one yet, please follow the instructions of exercise 0)


## Exercises

- [Exercise 0 - Getting Guided Experience System access](exercises/ex0/)
- [Exercise 1 - First Exercise Description](exercises/ex1/)
    - [Exercise 1.1 - Exercise 1 Sub Exercise 1 Description](exercises/ex1#exercise-11-sub-exercise-1-description)
    - [Exercise 1.2 - Exercise 1 Sub Exercise 2 Description](exercises/ex1#exercise-12-sub-exercise-2-description)
- [Exercise 2 - Second Exercise Description](exercises/ex2/)
    - [Exercise 2.1 - Exercise 2 Sub Exercise 1 Description](exercises/ex2#exercise-21-sub-exercise-1-description)
    - [Exercise 2.2 - Exercise 2 Sub Exercise 2 Description](exercises/ex2#exercise-22-sub-exercise-2-description)

  
**OR** Link to the Tutorial Navigator for example...

Start the exercises [here](https://developers.sap.com/tutorials/abap-environment-trial-onboarding.html).

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
