# Exercise 2 - Generation of Workflow
In this exercise, you will __generate a workflow__ for the Integration scenario - __SAP Build Setup (CLM Day 2025)__.

## Access the Cloud Integration Automation Service

* Click on the [BTP Global Account](https://emea.cockpit.btp.cloud.sap/cockpit/?idp=clm-day-01.accounts.ondemand.com#/globalaccount/9d88d4f5-c80a-4986-8a56-dbf4b7b5a223)
* Click on the Subaccount
  ![subaccount](../images/subaccount.png)
* Click on **Services > Instances and Subscriptions**
* Click on the icon against Cloud Integration Automation service to launch the application
* ![cias](../images/cias.png)


## Plan for Integration

Select the Plan for Integration tile in the Home screen of the CIAS application

1. You have lauched the application for Cloud Integration Automation Service


2. Select the __Plan for Integration__ tile in the home screen of the Cloud Integration Automation Service application.
   
![scenario selection](../images/plan_handson_1.png)


3. Search for **SAP Build Setup (CLM Day 2025)** integration scenario.

![scenario selection](../images/plan_handson_2.png)


4. Select the line item. It will open up the side panel with more information about the integration scenario.



5. Click on the Select Systems button in the side panel
   


6.	Click on the **SAP Business Technology Platform** system tile and search **CIAS EU Global Consumer**, and choose the tenant from the table.

![BTP](../images/plan_handson_5.png)

  
7.	Click on the **SAP BTP Identity Authentication Service** system tile and search **clm-day-01**, and choose the tenant from the below table.

![SCI](../images/plan_handson_6.png)


1. Click the **Generate Workflow** button on the top right corner, and choose **Background Execution** option.

![S4HC](../images/plan_handson_7.png)

9.	Press the **Proceed** button in the popup. 

![Generate](../images/plan_handson_8.png)

10. In **Verify System Details** screen, the selected system details can be verified and then press **Next Step** button. 

![Generate](../images/plan_handson_9.png)

11. In the **Scope Selection** screen, the scope of the execution can be reviewed and then press **Next Step** button.

![Generate](../images/plan_handson_10.png)

12. In the **Add Task Parameters** screen provide the values only for the below parameters and keep rest of the parameter values as is-:

**SAP Build Administrator** -: userXX@sapclm.org

**Subaccount Region** -: Europe Frankfurt eu10

**Subaccount Display Name** :  SAP CLM DAY USER XX 

**Subaccount Subdomain Name** – sap-clm-day-user-xx


<span style="color:red">**Note**</span> - replace **XX** in above parameter values with your user number 

![Generate](../images/plan_handson_11.png)

13. In this screen, press **Confirm** button to generate a workflow.
    
![Generate](../images/plan_handson_12.png)

## Result

You’ve now _successfully_ **generated the workflow**. Now click on the link to navigate to **Scenario Monitoring application**.

![Generate](../images/plan_handson_13.png)




In the next exercise, we will execute the workflow and complete the integration setup.

**Continue to - [Exercise 3 - Monitoring Configuration Setup](../ex3/README.md)**
