---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e249873ad28dd8532ec12fde7a7f6e07654e2b34
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests["{governanceRoleAssignmentRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```