---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3899f2754feb57fc962f7ffe449e8dbd893f50a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341365"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        EndpointType = "default"
        Identity = @{
            User = @{
                Id = "550fae72-d251-43ec-868c-373732c2704f"
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
                DisplayName = "Heidi Steen"
            }
        }
        LanguageId = "languageId-value"
        Region = "region-value"
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```