---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0f010d3d52f45ffe3731627959700064bc0f72f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106763"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserCalendarView -UserId $userId -Startdatetime "2017-01-01T19:00:00-08:00" -Enddatetime "2017-01-07T19:00:00-08:00" 

```