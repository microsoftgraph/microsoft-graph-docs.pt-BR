---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df16ef7709dcc73abdeb7a801db341b5f1edb1b8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests["{unifiedRoleEligibilityScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```