# Exercise 1 - Replicate CDS Views from SAP S/4HANA via Replication Flows to SAP Datasphere

Step by Step Solution guide:
Refer to the provided solution below for a detailed, step-by-step guide to complete Exercise 1
1.	Open your SAP Datasphere using the provided credentials. Your user is associated with space having same name as user where you can work and create your data artifacts.
   
    ![ex_01_01](images/ex_01_01.png)

2.	Click on Data Builder to see the Databuilder home page as shown below and scroll the horizontal scroll bar to the middle until you see “New Replication Flow” tile.
   
    ![ex_01_02](images/ex_01_02.png)

3.	Click on “New Replication Flow” tile to launch creation of new replication flow.
   
    ![ex_01_03](images/ex_01_03.png)

4.	Click on “Select Source Connection” button that launches a popup to select the source connection.

    ![ex_01_04](images/ex_01_04.png)

5.	Select S4_HANA which is of ABAP type from the list of connections. It will update the connection and “Select Source Container” button is auto selected for next step.

    ![ex_01_05](images/ex_01_05.png)

6.	Click on “Select Source Container” button and it launches “Select Container” popup. Then click on CDS – CDS Views Container.

    ![ex_01_06](images/ex_01_06.png)

7.	On selecting the CDS – CDS Views, you will see that the container is updated in Replication Flow screen and the “Add Source Objects” button is selected.

    ![ex_01_07](images/ex_01_07.png)

8.	Click on “Add Source Objects” button that launches “Select Source Objects” popup as shown below. Select “TMP – Local Objects” and then enter Z_CDS in search bar and click enter to see the required CDS views as shown. Select the CDS Views as shown.

    ![ex_01_08](images/ex_01_08.png)

9.	Click on Next button to see updated popup

    ![ex_01_09](images/ex_01_09.png)

10.	Click on Add Selection that shows that starts the fetching of source objects details from source

    ![ex_01_10](images/ex_01_10.png)

11.	All the 4 source objects details are fetched and shown as below

    ![ex_01_11](images/ex_01_11.png)

12.	No Projections are required here and hence you can skip that. Click on icon adjacent to “Select Target Connection”. It shows below popup to select target connection.

    ![ex_01_12](images/ex_01_12.png)

13.	Click on “SAP Datasphere”. It shows the new tables which are replicas of source objects and will be created in Datasphere.

    ![ex_01_13](images/ex_01_13.png)

14.	Select each of the target objects and update the Load Type to “Initial and Delta”. Repeat the same for all the target objects.

    ![ex_01_14](images/ex_01_14.png)

15.	For each target object, select on menu icon adjacent and rename Z_CDS_EPM_PO to Products, Z_CDS_EPM_SO to SalesOrders, Z_CDS_EPM_SO_I to SalesOrderItems and Z_CDS_EPM_BUPA to BusinessPartners.

    ![ex_01_15](images/ex_01_15.png)

16.	Click on Deploy icon in the general tab on top that launches Save popup with default name. Set the business name as “Inbound Repflow” which will automatically set technical name as “Inbound_RepFlow”.
    
    ![ex_01_16](images/ex_01_16.png)

17.	Click on Save button. It will start deploying. Check for the status in Properties Panel. The status is shown as “Not Deployed” initially and will get updated to “Deployed” after few seconds.

    ![ex_01_17](images/ex_01_17.png)

18.	Once the status is Deployed, click on run icon in the General tab above. You will see the Run Status in property panel getting updated to “Running”.

    ![ex_01_18](images/ex_01_18.png)

19.	Click on Monitor icon in Run Status tab in property panel to navigate to Monitoring which shows the status of replication objects as “Initial Running” or Retrying

    ![ex_01_19](images/ex_01_19.png)

20.	Wait until all the 4 replication objects are run for once (both initial and “initial and delta”) and be in retrying state waiting for any new data to arrive in source objects. Post this, you can check the tables in Table editor and check the preview to see data has come.

This concludes the Exercise 1 where the objective is to replicate data from S4 Hana source into Datasphere.
