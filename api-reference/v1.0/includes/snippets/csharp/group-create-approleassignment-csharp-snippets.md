---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15460ed6dad2fbc02719f5034405937551b268e1
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.Groups["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```