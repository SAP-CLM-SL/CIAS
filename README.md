# CLM Day 2026 - Automate SAP Build Setup and Innovate with Your First Custom AI Agent Using Cloud Integration Automation Service

## Overview

This session introduces participants to the **Cloud Integration Automation Service**, where you will gain hands-on experience implementing automated scenarios on **SAP BTP**. The hands-on is split into two parts:

- **Part 1** – **CLM Day 2026 Part 1 - Provision SAP Build services and create a custom Joule agent**: provision SAP Build services and create a custom **Joule agent** that helps maintenance planners validate whether a maintenance order can be fulfilled based on current material stock.
- **Part 2** *(Optional — if time permits)* – **CLM Day 2026 Part 2 - Set up a SAP Fiori launchpad site in SAP Build Work Zone and publish apps to it**: build a **SAP Fiori launchpad site** using SAP Build Work Zone, standard edition.

**<ins>Scenario Description</ins>**

Cloud Integration Automation Service simplifies and automates the technical setup of SAP Build — a comprehensive solution for business application development and automation. Rather than configuring each service manually, Cloud Integration Automation Service handles the end-to-end provisioning on SAP BTP, enabling teams to focus on building value instead of managing infrastructure.

As part of this setup, Cloud Integration Automation Service provisions a set of core SAP Build services on SAP BTP. It also provisions SAP Build Process Automation and SAP Joule to enable **Joule Studio**, where you can create and deploy custom AI agents. In this hands-on, you will build a custom agent as a practical example of what becomes possible after the automated setup is complete.

Cloud Integration Automation Service also provisions SAP Build Work Zone, standard edition, which can be used to create a SAP Fiori launchpad site.

![overview](images/overview.png)

**<ins>Configuration of the scenario with Cloud Integration Automation Service</ins>**

In this hands-on session, Cloud Integration Automation Service provisions the following services on SAP Business Technology Platform and sets up integration with SAP Cloud Identity Service. As a final step, you will use **Joule Studio** to build a custom agent and explore one of the outcomes of the automated setup.

## Services Provisioned in SAP BTP

- SAP Build Work Zone, standard edition
- SAP Build Process Automation
- SAP Build Apps
- SAP Task Center
- SAP Business Application Studio
- SAP Joule

![cias_overview](images/overview2.png)

## Required Systems & Services

- [x] __Cloud Integration Automation Service__: BTP Service used to set up the technical configuration of the integration scenario involving the below systems.
- [x] __SAP BTP Global Account__
- [x] __Cloud Identity Authentication Service__

## Access Information

You can log in to the above application/tenants with credentials assigned to you. 

1. __Username:__ Use the following email ID (`XX will be assigned to you during the hands-on exercise`)

    ```
    userXX@sapclm.org
    ```

2. __Password:__ Use the following password

    ```
    The password will be provided to you during the hands-on session
    ```

**NOTE:** While logging in to any of the above systems/tenants (**OPTIONAL**), select the **clm-day-01.accounts.ondemand.com** IDP (if prompted).

![Teched IDP](images/idp_login.png)

## Exercises

- [Exercise 1 - Overview of Cloud Integration Automation Service](ex1/README.md)
- [Exercise 2 - Generate the Workflow](ex2/README.md)
- [Exercise 3 - Monitor and Complete the Setup](ex3/README.md)

Once you complete the above exercises, you will have provisioned and configured services on BTP using Cloud Integration Automation Service and created a custom Joule agent in Joule Studio.

> **What's next?** You can run **Part 2** of this hands-on to create a SAP Fiori launchpad site using SAP Build Work Zone, standard edition.

> **Further Reading:** Curious about the data behind the agent? See [About the Sample Maintenance Backend](info/README.md) for the data model, entity descriptions, and sample prompts to try.


## Resources
1. [Cloud Integration Automation Service Discovery center](https://discovery-center.cloud.sap/serviceCatalog/cloud-integration-automation?region=all&service_plan=standard&commercialModel=cloud)
2. [SAP Help Portal](https://help.sap.com/docs/cloud-integration-automation/user-guide/overview?locale=en-US)
3. [SAP BTP Global Account](https://emea.cockpit.btp.cloud.sap/cockpit/?idp=clm-day-01.accounts.ondemand.com#/globalaccount/9d88d4f5-c80a-4986-8a56-dbf4b7b5a223) tenant used during the hands-on session.


## Code of Conduct
Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## How to obtain support
Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
