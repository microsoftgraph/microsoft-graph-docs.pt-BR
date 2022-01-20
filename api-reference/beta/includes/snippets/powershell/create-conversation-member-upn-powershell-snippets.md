---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 877814fe10aba7bf88406d0b4ede5926e4dc772d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121391"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    "User@odata.bind" = "https://graph.microsoft.com/beta/users/jacob@contoso.com"
    VisibleHistoryStartDateTime = [System.DateTime]::Parse("2019-04-18T23:51:43.255Z")
    Roles = @(
        "owner"
    )
}

New-MgChatMember -ChatId $chatId -BodyParameter $params

```