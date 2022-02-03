---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02d8d492585eacf86bd6fd2703b3897f49011617
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351266"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Sports"
    )
}

# A UPN can also be used as -UserId.
Update-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId -BodyParameter $params

```