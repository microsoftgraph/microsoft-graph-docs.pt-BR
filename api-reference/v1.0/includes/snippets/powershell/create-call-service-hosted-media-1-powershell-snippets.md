---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cea82e5a1316bd05b7eb064c3c414fbc62b3216
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136570"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    "@odata.type" = "#microsoft.graph.call"
    CallbackUri = "https://bot.contoso.com/callback"
    Targets = @(
        @{
            "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
            Identity = @{
                "@odata.type" = "#microsoft.graph.identitySet"
                User = @{
                    "@odata.type" = "#microsoft.graph.identity"
                    DisplayName = "John"
                    Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
                }
            }
        }
    )
    RequestedModalities = @(
        "audio"
    )
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
    }
}

New-MgCommunicationCall -BodyParameter $params

```