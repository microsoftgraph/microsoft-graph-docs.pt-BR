---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8ecffede3feba9421ccaa9a8bf58f5e6eec0ced
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350421"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Personal Tasks"
}

# A UPN can also be used as -UserId.
Update-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```