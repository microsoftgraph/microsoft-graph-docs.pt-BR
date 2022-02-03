---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eca9fd741c64cece3e64458a8195800e551df320
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339422"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    BusinessPhones = @(
        "+1 425 555 0109"
    )
    OfficeLocation = "18/2111"
}

# A UPN can also be used as -UserId.
Update-MgUser -UserId $userId -BodyParameter $params

```