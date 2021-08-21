---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 614705e4f6afe8c293adf9ad6c625f5d8dc131bf6e2f75cf36d2e5748cab6b96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = new PrivilegedRoleAssignment
{
    UserId = "userId-value",
    RoleId = "roleId-value"
};

await graphClient.PrivilegedRoleAssignments
    .Request()
    .AddAsync(privilegedRoleAssignment);

```