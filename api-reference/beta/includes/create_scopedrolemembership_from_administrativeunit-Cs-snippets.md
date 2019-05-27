---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 276762a7a7b55f4ec687e78b55aa52aba3ef3ee0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = new ScopedRoleMembership
{
    RoleId = "roleId-value",
    RoleMemberInfo = new Identity
    {
        Id = "id-value"
    }
};

await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers
    .Request()
    .AddAsync(scopedRoleMembership);

```