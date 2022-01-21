---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae458b97e6273ff5f84582d3b9c68dd6ae65e1c8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118981"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "menu.txt"
    ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}

New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```