---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8193db68562487a3d896f65e9eb476a875631442
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087750"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    Roles = @(
        "owner"
    )
    "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
}

New-MgTeamMember -TeamId $teamId -BodyParameter $params

```