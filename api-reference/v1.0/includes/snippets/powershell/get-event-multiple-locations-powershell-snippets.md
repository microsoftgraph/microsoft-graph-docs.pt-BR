---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1ada9c5f6885f454fbc2acbcb776af85d1e792a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136195"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,body,bodyPreview,organizer,attendees,start,end,location,locations" 

```