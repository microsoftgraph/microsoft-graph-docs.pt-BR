---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63f4de55c3e84341949a914c73d9864b87f21b61
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109409"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "name-value"
}

Update-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```