---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da1870b02fbf02aa52e7602cdfcfe39260c6a7ea
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339652"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Value = @(
        "externalId-value1"
        "externalId-value2"
    )
}

Remove-MgSecurityTiIndicatorByExternalId -BodyParameter $params

```