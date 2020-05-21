---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 757bb8059d0ca7b394777acd6f652d6c1c55ebec
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.Users["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```