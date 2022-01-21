---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b707efe1d1d512fd01826d2004c21be1a2f8a6d9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118967"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    ResponseStatus = @{
        Response = ""
        Time = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    }
    Recurrence = $null
    Uid = "iCalUId-value"
    ReminderMinutesBeforeStart = 99
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
    IsReminderOn = $true
    HideAttendees = $false
    Categories = @(
        "Red category"
    )
}

Update-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```