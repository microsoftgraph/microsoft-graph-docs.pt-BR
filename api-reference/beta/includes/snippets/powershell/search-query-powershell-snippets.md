---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 297b5b1db69a13a4d534801ada78f9ee641c2ddf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348814"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Requests = @(
        @{
            EntityTypes = @(
                "externalItem"
            )
            ContentSources = @(
                "/external/connections/connectionfriendlyname"
            )
            Query = @{
                QueryString = "contoso product"
            }
            From = 0
            Size = 25
            Fields = @(
                "title"
                "description"
            )
        }
    )
}

Invoke-MgQuerySearch -BodyParameter $params

```