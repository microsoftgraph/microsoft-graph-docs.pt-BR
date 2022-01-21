---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf7f2e93301a76ab5a09290a169a9d353ccba1a0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101578"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#Microsoft.Graph.channel"
    MembershipType = "private"
    DisplayName = "My First Private Channel"
    Description = "This is my first private channels"
    Members = @(
        @{
            "@odata.type" = "#microsoft.graph.aadUserConversationMember"
            "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
            Roles = @(
                "owner"
            )
        }
    )
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```