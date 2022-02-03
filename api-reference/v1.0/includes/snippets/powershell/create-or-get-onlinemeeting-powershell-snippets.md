---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 626c275a2b0f55f86224cf59823e96c916ec651f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345781"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    StartDateTime = [System.DateTime]::Parse("2020-02-06T01:49:21.3524945+00:00")
    EndDateTime = [System.DateTime]::Parse("2020-02-06T02:19:21.3524945+00:00")
    Subject = "Create a meeting with customId provided"
    ExternalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56"
    Participants = @{
        Attendees = @(
            @{
                Identity = @{
                    User = @{
                        Id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                }
                Upn = "test1@contoso.com"
            }
        )
    }
}

# A UPN can also be used as -UserId.
Invoke-MgCreateOrGetUserOnlineMeeting -UserId $userId -BodyParameter $params

```