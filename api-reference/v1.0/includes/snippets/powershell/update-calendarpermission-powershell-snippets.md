---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 977364be6e79d37900ba5f957f35d2f372a00c4f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124925"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Role = "write"
}

Update-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId -BodyParameter $params

```