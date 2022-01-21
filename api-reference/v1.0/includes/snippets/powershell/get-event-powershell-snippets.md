---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a73dad9e7453161bb0226c26b476184d090c8d38
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136194"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees" 

```