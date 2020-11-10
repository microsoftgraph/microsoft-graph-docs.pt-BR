---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33f5baf164ea96e5e1ddbfc58174c3be85c5ec98
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951736"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5";
accessPackageResourceRequest.requestType = "AdminAdd";
accessPackageResourceRequest.justification = "";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.displayName = "Sales";
accessPackageResource.description = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.url = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.resourceType = "SharePoint Online Site";
accessPackageResource.originId = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.originSystem = "SharePointOnline";
accessPackageResourceRequest.accessPackageResource = accessPackageResource;

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```