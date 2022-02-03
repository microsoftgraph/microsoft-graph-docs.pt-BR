---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7aba270395c197ae75ccadd7cd07dfa710924cef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345666"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Schedules = @(
        "adelev@contoso.onmicrosoft.com"
        "meganb@contoso.onmicrosoft.com"
    )
    StartTime = @{
        DateTime = "2019-03-15T09:00:00"
        TimeZone = "Pacific Standard Time"
    }
    EndTime = @{
        DateTime = "2019-03-15T18:00:00"
        TimeZone = "Pacific Standard Time"
    }
    AvailabilityViewInterval = 60
}

# A UPN can also be used as -UserId.
Get-MgUserDefaultCalendarSchedule -UserId $userId -BodyParameter $params

```