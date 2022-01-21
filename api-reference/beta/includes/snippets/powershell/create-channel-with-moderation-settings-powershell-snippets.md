---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 765b585c5e74e08e66518756e11adf8c14bde172
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131561"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "TestChannelModeration"
    Description = "Test channel moderation."
    MembershipType = "standard"
    ModerationSettings = @{
        UserNewMessageRestriction = "everyoneExceptGuests"
        ReplyRestriction = "everyone"
        AllowNewMessageFromBots = $true
        AllowNewMessageFromConnectors = $true
    }
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```