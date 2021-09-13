---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49946957cb52f33d367318cbb107b0c9a83331c98f3a62f4e70df16a27e0bef1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101103"
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

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers
    .Request()
    .AddAsync(scopedRoleMembership);

```