---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b427e4e9f7ebf245de4c2de429b5cbd169dad6aa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351435"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does noon work for you?"
    }
    Start = @{
        DateTime = "2017-04-15T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2017-04-15T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "samanthab@contoso.onmicrosoft.com"
                Name = "Samantha Booth"
            }
            Type = "required"
        }
    )
    AllowNewTimeProposals = $true
    TransactionId = "7E163156-7762-4BEB-A1C6-729EA81755A7"
}

# A UPN can also be used as -UserId.
New-MgUserEvent -UserId $userId -BodyParameter $params

```