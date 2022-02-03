---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6d4da4aafac6d917cb0391cbeb61d9455d447bc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348188"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    AtAprovedLocation = $true
    Notes = @{
        ContentType = "text"
        Content = "clock out smaple notes"
    }
}

Invoke-MgClockTeamScheduleTimeCardOut -TeamId $teamId -TimeCardId $timeCardId -BodyParameter $params

```