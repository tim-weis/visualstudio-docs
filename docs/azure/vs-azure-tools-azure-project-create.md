---
title: Create an Azure cloud service project
description: Learn now to create an Azure cloud service project with Visual Studio
author: ghogen
manager: jmartens
ms.subservice: azure-development
ms.topic: how-to
ms.date: 03/19/2019
ms.author: ghogen
---
# Create an Azure cloud service project with Visual Studio

 [!INCLUDE [Cloud Services](./includes/cloud-services-legacy.md)]

Visual Studio provides a project template that lets you create an [Azure cloud service](/azure/cloud-services/cloud-services-choose-me), which is a simple general-purpose Azure service. Once the project has been created, Visual Studio enables you to configure, debug, and deploy the cloud service to Azure.

## Prerequisites

- [!INCLUDE [prerequisites-azure-subscription](includes/prerequisites-azure-subscription.md)]

## Steps to create an Azure cloud service project in Visual Studio
This section walks you through creating an Azure cloud service project in Visual Studio with one or more web roles.

1. From the start window, choose **Create a new project**.

1. In the search box, type in *Cloud*, and then choose **Azure Cloud Service**.

   ![New Azure cloud service](./media/vs-azure-tools-azure-project-create/vs-2019/new-project-cloud-service.png)

1. Give the project a name and choose **Create**.

   ![Give the project a name](./media/vs-azure-tools-azure-project-create/vs-2019/new-project-cloud-service-2.png)
1. In the **New Microsoft Azure Cloud Service** dialog, select the roles that you want to add, and choose the right arrow button to add them to your solution.

    ![Select new Azure cloud service roles](./media/vs-azure-tools-azure-project-create/new-cloud-service.png)

1. To rename a role that you've added, hover on the role in the **New Microsoft Azure Cloud Service** dialog, and, from the context menu, select **Rename**. You can also rename a role within your solution (in the **Solution Explorer**) after it has been added.

    ![Rename Azure cloud service role](./media/vs-azure-tools-azure-project-create/new-cloud-service-rename.png)

The Visual Studio Azure project has associations to the role projects in the solution. The project also includes the *service definition file* and *service configuration file*:

- **Service definition file** - Defines the run-time settings for your application, including what roles are required, endpoints, and virtual machine size.
- **Service configuration file** - Configures how many instances of a role are run and the values of the settings defined for a role.

For more information about these files, see [Configure the Roles for an Azure cloud service with Visual Studio](vs-azure-tools-configure-roles-for-cloud-service.md).

## Next steps
- [Managing roles in Azure cloud service projects with Visual Studio](./vs-azure-tools-cloud-service-project-managing-roles.md)
