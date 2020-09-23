---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5eea52d59b52032327cab608bdf068370a916bcd
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223428"
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

await graphClient.Directory.AdministrativeUnits["{id}"].ScopedRoleMembers
    .Request()
    .AddAsync(scopedRoleMembership);

```