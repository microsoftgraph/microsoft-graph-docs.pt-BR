---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15317e4fe298f8aa28e1c54793b5361eefabb548
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112674"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.itemAttachment"
    Name = "Holiday event"
    Item = @{
        "@odata.type" = "microsoft.graph.event"
        Subject = "Discuss gifts for children"
    }
}

New-MgUserOutlookTaskAttachment -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```