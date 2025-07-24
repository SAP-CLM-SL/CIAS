# Exercise 3 - Monitoring Configuration Setup
In this exercise, we will **monitor** the progress of the automated setup and verify the automations.

## Scenario Monitoring

Select the Plan for Integration tile in the Home screen of the CIAS application

1.	The real time status of the execution can be seen in this application. You can see that the task **Create SAP BTP Subaccount** is in status **Executing Automation**.
   ![scenario selection](../images/monitoring_handson_1.png)

2.	Once the task **Create SAP BTP Subaccount** is in **Completed status**, a new subaccount would have been created in the SAP BTP Global Account- CIAS EU Global Consumer that you had previously selected in the Planning screen.
   
  ![scenario selection](../images/monitoring_handson_2.png)


3.	To  check the newly created subaccount, you can log in to the SAP BTP Global Account- CIAS EU Global Consumer . The email and password is the same as mentioned in the Access Information. 

  ![scenario selection](../images/monitoring_handson_3.png)


4.	You can see the newly created subaccount in the global account..

  ![scenario selection](../images/monitoring_handson_4.png)


5.	In the **Scenario Monitoring** application, the following tasks will be executing sequentially. You can see the status in the Tasks table. Wait for the below listed tasks to be executed successfully.

   | Task ID      | Task Description                                              |
   |-----------|---------------------------------------------------------------|
   | A00005    | Create SAP BTP Subaccount                                     |
   | A00006    | Enable Cloud Foundry Environment                              |
   | A00007    | Create Space                                                  |
   | A00008    | Establish Trust with IAS                                      |
   | A00009    | Create Destination and XSUAA services                         |
   | A00010    | Disable Default IDP                                           |
   | A00011    | SAP Build Work Zone, standard edition Entitlement             |
   | A00012    | Activate SAP Build Work Zone, standard edition                |
   | A00013    | Assign Role Collection for SAP Build Work Zone, standard edition |
   | A00014    | SAP Build Work Zone, advanced edition Entitlement             |
   | A00015    | Activate SAP Build Work Zone, advanced edition                |
   | A00016    | Assign Role Collection for SAP Build Work Zone, advanced edition |
   | A00017    | Create Destination for SAP Build Work Zone Content            |
   | A00018    | SAP Task Center Entitlement                                   |
   | A00019    | Activate SAP Task Center                                      |
   | A00020    | Assign Role Collection for SAP Task Center                    |
   | A00021    | Create Destinations for SAP Task Center                       |
   | A00022    | SAP Build Apps Entitlement                                    |
   | A00023    | Activate SAP Build Apps                                       |
   | A00024    | Assign Role Collection for Build Apps                         |
   | A00025    | SAP Build Process Automation Entitlement                      |
   | A00026    | Activate SAP Build Process Automation                         |
   | A00027    | Assign Role Collection for SAP Build Process Automation       |
   | A00028    | Create Destinations for SAP Business Process Automation       |
   | A00029    | SAP Business Application Studio Entitlements                  |
   | A00030    | Activate SAP Business Application Studio                      |
   | A00031    | Assign Role Collection for SAP Business Application Studio    |


6.	Click on the **SAP Business Technology Platform** system tile and search **CIAS EU Global Consumer**, and choose the tenant from the table.

![BTP](../images/monitoring_handson_5.png)

  
7.	Click on the **SAP BTP Identity Authentication Service** system tile and search **clm-day-01**, and choose the tenant from the below table.

![SCI](../images/monitoring_handson_6.png)


8. Click the **Generate Workflow** button on the top right corner, and choose **Background Execution** option.

![S4HC](../images/monitoring_handson_7.png)

9.	Press the **Proceed** button in the popup. 

![Generate](../images/monitoring_handson_8.png)

10. In **Verify System Details** screen, the selected system details can be verified and then press **Next Step** button. 

![Generate](../images/monitoring_handson_9.png)

11. In the **Scope Selection** screen, the scope of the execution can be reviewed and then press **Next Step** button.

![Generate](../images/monitoring_handson_10.png)

12. In the **Add Task Parameters** screen provide the values only for the below parameters and keep rest of the parameter values as is-:

**SAP Build Administrator** -: userXX@sapclm.org

**Subaccount Region** -: Europe Frankfurt eu10

**Subaccount Display Name** :  SAP CLM DAY USER XX 

**Subaccount Subdomain Name** – sap-clm-day-user-xx


<span style="color:red">**Note**</span> - replace **XX** in above parameter values with your user number 

![Generate](../images/monitoring_handson_11.png)

13. In this screen, press **Confirm** button to generate a workflow.
    
![Generate](../images/monitoring_handson_12.png)

## Result

You’ve now _successfully_ **generated the workflow**. Now click on the link to navigate to **Scenario Monitoring application**.

![Generate](../images/monitoring_handson_13.png)




In the next exercise, we will execute the workflow and complete the integration setup.

**Continue to - [Exercise 3 - Monitoring Configuration Setup](../ex3/README.md)**
