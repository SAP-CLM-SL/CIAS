
# Exercise 1: Getting Started

In this exercise, you will get an overview of the capabilities of CIAS which will be helpful for the successful completion of the hands-on exercise.

## Overview

The Cloud Integration Automation Service homepage consists of three tiles:

### 1. Plan Integration Scenarios

**Choose and plan for an integration scenario**

This section contains the integration scenarios that are onboarded into CIAS. You can choose based on the Cloud or Hybrid setup and generate a workflow. It has an integrated landscape discovery that prompts you to select the systems you own. In the case of a fully automated scenario, you can run the whole setup in the background as well.

**Note: In the next exercise, we will take a deeper look into the functions of the Planning app.**

![plan](../images/plan_overiew_1.png)

### 2. My Inbox

**View and manage all the integration tasks assigned to you**

The Inbox feature in Cloud Integration Automation Service supports workflow execution by automatically delegating tasks based on user authorization and scope. Its integrated parameter management system minimizes errors and ensures seamless integration by pre-populating task parameters from preceding tasks. Furthermore, its automation capabilities eliminate manual operations, thereby boosting efficiency and reducing potential human errors.

![inbox](../images/plan_overiew_2.png)

The following tabs are available within the Inbox:

1. **Task Instructions** - Displays the documentation for the current task, including configuration parameters and automation controls.
2. **Overview** - Provides a hierarchical view of all the tasks and their documentation for the complete workflow. **Note:** This view is for reference only. Always use the **Task Instructions** tab to act on the current task.
3. **Comments** - Allows you to add comments to communicate with other workflow users for the current workflow.
4. **System Access** - Provides information about the system associated with the current task.
5. **Assigned Users** - Shows workflow user information for the current task.
6. **Support Information** - Contains metadata about the workflow.
7. **Logs** - After triggering an automation, view execution logs here. Individual automation logs appear next to each parameter section; use the **Logs** button at the top right for aggregate logs.

![task overview](../images/plan_overiew_3.png)

#### Task Execution in Inbox

There are 2 kinds of workflow tasks you may encounter while executing a workflow in Inbox.

#### 1. Automation task

Automation tasks perform the configuration automatically based on the parameters **(1)** provided. You have two ways to run the automation:

- **Start Automation (2a)** — triggers the automation interactively. The status badge **(3)** next to the parameter section updates as the automation runs. Once it completes, choose **Complete Task (4)** to move to the next task.
- **Continue (2b)** — runs the automation in the background and automatically completes the task when done. No further action is needed.

The **Manual Instructions** section below the parameters serves as an alternative if the automation cannot be used.

**For the hands-on session, in case of an error, please reach out to colleagues for support.**

![Automation task](../images/plan_overiew_4.png)

#### 2. Manual task

Manual tasks require you to perform the configuration steps yourself. They may contain a **parameter** section **(1)** — for example, a file to download — but there is no Start Automation button. The **Manual Instructions** section contains **deep links (2)** that open the relevant system or page directly. Follow the steps described, using those links to navigate. Once you have completed all the steps, choose **Complete Task (3)** to proceed to the next task.

![Manual task](../images/plan_overiew_5.png)


### 3. Monitor Integration Scenarios

**Track the progress for all the integration scenarios**

Monitor Integration Scenarios provides a comprehensive view of all workflow instances running in this tenant. It shows each integration scenario, the tasks within it, and their current progress and status. Use this tile to track execution and verify that automated tasks have completed successfully.

![seo](../images/plan_overiew_6.png)

Let us now proceed to the next exercise, where we will generate the workflow.

**Continue to - [Exercise 2 - Generate a workflow](../ex2/README.md)**
