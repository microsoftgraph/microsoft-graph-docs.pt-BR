---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c66076ffe79facf8c48967b0cc529f48bdfab4af
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352016"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,body,bodyPreview" 

```