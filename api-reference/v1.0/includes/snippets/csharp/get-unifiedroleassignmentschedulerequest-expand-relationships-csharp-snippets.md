---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9838fd7a39f1310dca32d9d0d93ffc1b3abb2440
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Request()
    .Expand("roleDefinitionId")
    .Select("principalId,action,roleDefinitionId")
    .GetAsync();

```