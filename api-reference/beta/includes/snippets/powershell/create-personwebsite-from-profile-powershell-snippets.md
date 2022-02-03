---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc0ed9a58a12f4740a082057c59c683ab335af19
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351747"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "football"
    )
    DisplayName = "Lyn Damer"
    WebUrl = "www.lyndamer.no"
}

# A UPN can also be used as -UserId.
New-MgUserProfileWebsite -UserId $userId -BodyParameter $params

```