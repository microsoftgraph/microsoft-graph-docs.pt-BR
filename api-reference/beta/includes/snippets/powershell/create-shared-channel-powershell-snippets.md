---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee37a2ba4b1d881286efdd70293a5c9e7de5be1d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202774"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "My First Shared Channel"
    Description = "This is my first shared channel"
    MembershipType = "shared"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            "User@odata.bind" = "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')"
            Roles = @(
                "owner"
            )
        }
    )
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```