---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 027da56124a5f9085cb1d3776dde0ebf138e6bc6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345242"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    InputIds = @(
        "{rest-formatted-id-1}"
        "{rest-formatted-id-2}"
    )
    SourceIdType = "restId"
    TargetIdType = "restImmutableEntryId"
}

# A UPN can also be used as -UserId.
Invoke-MgTranslateUserExchangeId -UserId $userId -BodyParameter $params

```