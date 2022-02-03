---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 697ca8499d311c184b24c4635a849d7a090a101e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350547"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId

```