- Exercise 3 - Preparing Analytic Data set with historic and delta records.
  - Exercise 3.1 - Create an Analytical Dataset model with transformation flow generated target delta table.
  - Exercise 3.2 – Update source tables record in Data Maintenance editor.
  - Exercise 3.3 – Execute Transformation flow to pull the delta records from source.
  - Exercise 3.4 – Preview the Analytical dataset model to see the historical and latest pulled records from Transformation flow Delta local table.
 - Exercise 4 – Egress use case via replication flow.
   - Exercise 4.1 – Replication flow with inbound and outbound sources.

# Exercise 3 - Preparing Analytical Dataset with historic and delta records.
To create an analytical dataset model, you will need to create a graphical view model in the Data Builder. 
 So, let's get started then. These are the steps we are going to run through:
 
-	Exercise 3.1 - Create an Analytical Dataset model with transformation flow generated target delta table.
-	Exercise 3.2 – Update source tables record in Data Maintenance editor
-	Exercise 3.3 – Execute Transformation flow to pull the delta records from source.
-	Exercise 3.4 – Preview the Analytical dataset model to see the historical and latest pulled records from Transformation flow Delta local table

- ##	Exercise 3.1 - Create an Analytical Dataset model with transformation flow generated target delta table.

1. Open the Graphical view app from Data builder.
1. <img width="396" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/f600f4e0-9e3b-4220-823e-ccda18c1809d">
1. Create Graphical view of semantic type Analytical dataset with delta local table and source table.
1. <img width="387" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/1919d61f-2264-4cb3-809b-f75c8b28deb5">
1. Add Projection node on source table.
1. Below mentioned 2 columns expose in the projection node.
1. <img width="387" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/b02b59bd-7b91-4e1a-80c9-0f095e146031">
1. Perform inner join on projection node and delta local table and map the “PRODUCTID” key column.
1. Add calculation node with calculated column “InvoiceRebateperItem” with this expression “Historic_Sticker_Price - GROSSAMOUNT” and validate the expression. 
1. Go to the output node, Open properties panel. 
1. Go to attributes section, By this option change column to measure.
1. <img width="187" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/57671591-b65a-47ce-95d3-bf36934f6e07">
1. Add below mentioned columns in the measures.
1. <img width="224" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/fca89d5f-312f-47ba-a44a-6184d7ac28db">
1. Open Attributes dialog, by clicking on edit icon.
1. <img width="184" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/8032eabd-c083-4f4c-97fd-320408aefa93">
1. Set the semantic type (Currency code and Unit of Measure) for below mentioned columns.
1. <img width="402" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/b1be2d30-8fa8-4fc7-b943-d67f607f7e86">
1. Deploy the view.
1. Perform data preview by clicking on context menu preview icon.
1. <img width="391" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/a1bb508b-dac0-4f7c-b4d2-a21f2f18686b">
1. Launch preview settings, by this icon.
1. <img width="137" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/b0f7ac70-7a7f-48e4-aeee-f4d098d2c1d1">
1. Apply filter on preview.
1. <img width="280" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/bf032c31-634c-4e2a-85bd-02c939011cca">
1. In the preview, historic sticker price and current sticker price for filtered productid.
1. <img width="355" alt="image" src="https://github.com/SAP-samples/teched2023-DA260/assets/147159572/4c6a2262-2e9f-422d-b311-cfa58772d2f9">


















 





