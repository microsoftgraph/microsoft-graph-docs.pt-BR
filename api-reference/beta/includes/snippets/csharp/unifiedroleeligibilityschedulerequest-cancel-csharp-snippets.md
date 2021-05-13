---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df16ef7709dcc73abdeb7a801db341b5f1edb1b8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests["{unifiedRoleEligibilityScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```