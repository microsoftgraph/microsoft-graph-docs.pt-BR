---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd948ac268f650b3b17f3ee7d2082eb2044847df
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348205"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    AtAprovedLocation = $true
    Notes = @{
        ContentType = "text"
        Content = "clock in notes"
    }
}

Invoke-MgClockTeamScheduleTimeCardIn -TeamId $teamId -BodyParameter $params

```