---
title: Use Azure Blockchain Workbench data in Microsoft Power BI
description: Learn how to load and view Azure Blockchain Workbench SQL DB data in Microsoft Power BI.
services: azure-blockchain
keywords:
author: PatAltimore
ms.author: patricka
ms.date: 5/3/2018
ms.topic: article
ms.service: azure-blockchain
ms.reviewer: mmercuri
manager: femila
---
# Using Azure Blockchain Workbench data with Microsoft Power BI

Microsoft Power BI provides the ability to easily generate powerful reports from SQL DB databases using Power BI Desktop and then publish them to [https://www.powerbi.com](http://www.powerbi.com).

This article contains a step by step walkthrough of how to connect to Azure Blockchain Workbench's SQL Database from within PowerBI desktop, create a report, and deploy the report to powerbi.com.

## Prerequisites

* Download [PowerBI Desktop](https://aka.ms/pbidesktopstore).

## Connecting PowerBI to data in Azure Blockchain Workbench

1.  Open Power BI Desktop.
2.  Select **Get Data**.

    ![Get data](media/blockchain-workbench-data-powerbi/get-data.png)
3.  Select **SQL Server** from the list of data source types.

4.  Provide the server and database name in the dialog. Specify if you want to import the data or perform a **DirectQuery**. Select **OK**.

    ![Select SQL Server](media/blockchain-workbench-data-powerbi/select-sql.png)

5.  Provide the database credentials to access Azure Blockchain Workbench. Select **Database** and enter your credentials.

    If you are using the credentials created by the Azure Blockchain Workbench deployment process, the username is **dbadmin** and the password is the one you provided during deployment.

    ![SQL DB settings](media/blockchain-workbench-data-powerbi/db-settings.png)

6.  Once connected to the database, the **Navigator** dialog displays the tables and views available within the database. The views are designed for reporting and are all prefixed **vw**.

    ![Navigator](media/blockchain-workbench-data-powerbi/navigator.png)

7.  Select the views you wish to include. For demonstration purposes, we include **vwContractAction**, which provides details on all of the actions that have taken place on a contract.

    ![Select views](media/blockchain-workbench-data-powerbi/select-views.png)

You can now create and publish reports as you normally would with Power BI.

## Next steps

> [!div class="nextstepaction"]
> [Database views in Azure Blockchain Workbench](blockchain-workbench-database-views.md)