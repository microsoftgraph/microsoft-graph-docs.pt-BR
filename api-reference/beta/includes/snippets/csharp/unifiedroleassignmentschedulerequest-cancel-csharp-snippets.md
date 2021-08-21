---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c2daf43e271994cda79de23e5c293be97911b63678413914b0496c638e7e2a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```