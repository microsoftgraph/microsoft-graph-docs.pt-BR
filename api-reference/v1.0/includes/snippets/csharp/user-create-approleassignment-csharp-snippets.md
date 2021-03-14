---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66503fceb166d8ab98ca5dbea2fd6963d9ffbcac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```