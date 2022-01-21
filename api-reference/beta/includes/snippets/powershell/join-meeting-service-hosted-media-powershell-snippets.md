---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c4ee18c94facf543eb598dbf128a525ca886e74
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119488"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    "@odata.type" = "#microsoft.graph.call"
    CallbackUri = "https://bot.contoso.com/callback"
    RequestedModalities = @(
        "audio"
    )
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
        PreFetchMedia = @(
        )
    }
    ChatInfo = @{
        "@odata.type" = "#microsoft.graph.chatInfo"
        ThreadId = "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2"
        MessageId = "0"
    }
    MeetingInfo = @{
        "@odata.type" = "#microsoft.graph.organizerMeetingInfo"
        Organizer = @{
            "@odata.type" = "#microsoft.graph.identitySet"
            User = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
                TenantId = "9f386a15-f9cc-445b-8106-ac85e314a07b"
                DisplayName = "Bob"
            }
        }
        AllowConversationWithoutHost = $true
    }
    TenantId = "86dc81db-c112-4228-9222-63f3esaa1edb"
}

New-MgCommunicationCall -BodyParameter $params

```