---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13b0a861e3b416ee8875a94970cd997863fd9c9d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349873"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Charity work"
}

# A UPN can also be used as -UserId.
Update-MgUserOutlookTaskFolder -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId -BodyParameter $params

```