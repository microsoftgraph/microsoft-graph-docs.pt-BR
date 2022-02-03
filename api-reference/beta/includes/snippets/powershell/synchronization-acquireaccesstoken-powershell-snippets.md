---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f3ab410f4844d6df26a4fa248fea9db8ecf391b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347070"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Credentials = @(
        @{
            "@odata.type" = "microsoft.graph.synchronizationSecretKeyStringValuePair"
        }
    )
}

Get-MgApplicationSynchronizationAccessToken -ApplicationId $applicationId -BodyParameter $params

```