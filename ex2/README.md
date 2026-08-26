# Exercise 2 - Generation of Workflow
In this exercise, you will __generate a workflow__ for the Integration scenario - __CLM Day 2026 Part 1 - Build Services and Joule Agent__.

## Access the Cloud Integration Automation Service

* Click on the <a href="https://emea.cockpit.btp.cloud.sap/cockpit/?idp=clm-day-01.accounts.ondemand.com#/globalaccount/9d88d4f5-c80a-4986-8a56-dbf4b7b5a223" target="_blank">BTP Global Account</a>
* Click on the Subaccount
  ![subaccount](../images/subaccount.png)
* Click on **Services > Instances and Subscriptions**
* Click on the icon against Cloud Integration Automation service to launch the application
  ![cias](../images/cias.png)

## Plan Integration Scenarios

1. On the Cloud Integration Automation Service home screen, select the **Plan Integration Scenarios** tile.

   ![scenario selection](../images/plan_handson_1.png)

2. On the **Integration Solutions and Scenarios** page, search for **CLM** in the search box. The **CLM Day Event - Hands-On Enablement** solution appears with both 2026 scenarios listed.

   ![scenario selection](../images/plan_handson_2.png)

3. Select **CLM Day 2026 Part 1 - Provision SAP Build services and create a custom Joule agent.** A panel opens on the right showing the scenario description and a **Scenario Options** dropdown.

   ![scenario selection](../images/plan_handson_3.png)

4. In the **Scenario Options** dropdown, ensure **Provision Build Services and Create a Joule Agent** is selected, then click **Start**.

   ![system selection](../images/plan_handson_4.png)

5. In the **Select Scope** step, three services are pre-selected and required to complete this hands-on: **SAP Build Process Automation** and **SAP Joule** (needed for Part 1), and **SAP Build Work Zone, standard edition** (needed for Part 2). Do not deselect these. The remaining services are optional — you may select additional ones if you would like to explore further. Click **Next Step** to continue.

   ![scope selection](../images/plan_handson_5.png)

6. In the **Select Systems** step, select the systems to be used for provisioning:
   - Click the value help icon **(1)** next to **SAP Business Technology Platform**, search for **CIAS EU**, and select **CIAS EU Global Consumer** **(2)**.
   - Click the value help icon **(3)** next to **SAP BTP Identity Authentication Service**, search for **clm-day-01**, and select **https://clm-day-01.accounts.ondemand.com** **(4)**.

   Once both systems are selected, click **Next Step**.

   ![system details](../images/plan_handson_6.png)

7. If a **Systems Details** popup appears warning about different landscapes, review the details and click **Proceed**.

   ![systems details popup](../images/plan_handson_7.png)

8. In the **Add Task Parameters** step, provide the following values and keep the rest as-is:

   **Subaccount Display Name (1):** JouleAgentXX

   **Subaccount Subdomain (2):** joule-agent-XX

   <span style="color:red">**Note**</span> - replace **XX** with your user number. Click **Next Step**.

   ![task parameters](../images/plan_handson_8.png)

9. In the **Review** step, check the disclaimer checkbox **(1)**, review the summary, and click **Finish**.

   ![review](../images/plan_handson_9.png)

## Result

You've now _successfully_ **generated the workflow**. The success screen shows your **Scenario Instance Name** and an **Integration Overview** summary. Click **Monitor Integration Setup** to navigate to the Monitor Integration Scenarios application and track progress.

![result](../images/plan_handson_10.png)

In the next exercise, we will monitor the workflow execution and complete the integration setup.

**Continue to - [Exercise 3 - Monitoring Configuration Setup](../ex3/README.md)**
