---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bd99831cd940652615ee6ce2d9899d8eb75d18d9f42986dfad604d7c55c1bde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassification = new DelegatedPermissionClassification
{
    PermissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
    PermissionName = "User.Read",
    Classification = PermissionClassificationType.Low
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].DelegatedPermissionClassifications
    .Request()
    .AddAsync(delegatedPermissionClassification);

```