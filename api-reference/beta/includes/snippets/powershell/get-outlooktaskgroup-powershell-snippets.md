---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcab6ffa5eb364f16f8d15d62b74c180c7934f53
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349978"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId

```