---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee8dce5f06527170c502d7702890cf16c1abb467
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351283"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "My Github contributions!"
    UserId = "innocenty.popov"
    Service = @{
        Name = "GitHub"
        WebUrl = "https://github.com"
    }
}

# A UPN can also be used as -UserId.
New-MgUserProfileWebAccount -UserId $userId -BodyParameter $params

```