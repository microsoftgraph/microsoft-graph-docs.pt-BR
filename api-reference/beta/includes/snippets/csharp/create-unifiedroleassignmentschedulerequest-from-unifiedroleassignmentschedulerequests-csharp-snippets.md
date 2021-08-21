---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 120cacfb7adcd76cf110b41ca70af454d28faceb64e44bf89cd3d90c3730bbc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = "String",
    PrincipalId = "String",
    RoleDefinitionId = "String",
    DirectoryScopeId = "String",
    AppScopeId = "String",
    IsValidationOnly = false,
    TargetScheduleId = "String",
    Justification = "String",
    ScheduleInfo = new RequestSchedule
    {
    },
    TicketInfo = new TicketInfo
    {
    }
};

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .AddAsync(unifiedRoleAssignmentScheduleRequest);

```