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
   
  ![system selection](../images/monitoring_handson_5.png)


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
