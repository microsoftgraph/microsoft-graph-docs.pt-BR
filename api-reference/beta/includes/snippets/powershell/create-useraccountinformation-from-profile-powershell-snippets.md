---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a01c4de2b645937c2b176ae430a8332bab4689e7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351456"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
    CountryCode = "NO"
}

# A UPN can also be used as -UserId.
New-MgUserProfileAccount -UserId $userId -BodyParameter $params

```