---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95cbd936372b73180fc1aa0ea0ee01aa4dce34c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119297"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    Roles = @(
        "owner"
    )
    "User@odata.bind" = "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
}

New-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```