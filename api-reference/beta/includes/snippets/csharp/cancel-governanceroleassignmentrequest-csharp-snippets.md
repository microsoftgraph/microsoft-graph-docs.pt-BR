---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f22d37104b59d9606e279455157c572ad72d5b6c95ca8fa44d5d9086b932b585
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests["{governanceRoleAssignmentRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```