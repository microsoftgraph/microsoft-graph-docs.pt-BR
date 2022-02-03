---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9788075a2c7b80c92d122c595401421e2ddca4e4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341046"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Complete-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId

```