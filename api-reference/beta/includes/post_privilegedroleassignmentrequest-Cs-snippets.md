---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4de6585f9984fb82ff12158bd477b98a2eaa85c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequest
{
    Duration = "2",
    Reason = "Activate the role for business purpose",
    TicketNumber = "234",
    TicketSystem = "system",
    Schedule = new GovernanceSchedule
    {
        StartDateTime = "2018-02-08T02:35:17.903Z"
    },
    EvaluateOnly = false,
    Type = "UserAdd",
    AssignmentState = "Active",
    RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
};

await graphClient.PrivilegedRoleAssignmentRequests
    .Request()
    .AddAsync(privilegedRoleAssignmentRequest);

```