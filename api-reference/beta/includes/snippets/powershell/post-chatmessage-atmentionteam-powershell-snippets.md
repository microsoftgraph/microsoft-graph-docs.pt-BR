---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 268e24de84791b112a9a7a87fad2080e73284543
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109441"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "<div><div><at id="0">GraphTesting</at>&nbsp;Hello team</div></div>"
    }
    Mentions = @(
        @{
            Id = 0
            MentionText = "GraphTesting"
            Mentioned = @{
                Conversation = @{
                    Id = "68a3e365-f7d9-4a56-b499-24332a9cc572"
                    DisplayName = "GraphTesting"
                    ConversationIdentityType = "team"
                }
            }
        }
    )
    Reactions = @(
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```