---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 824d5685a497f76d8831553f81765104bb926c3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101953"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "displayName-value"
    ApiVersion = 99
    Encryption = @{
        Protocol = "protocol-value"
        Secret = "secret-value"
    }
    IsActive = $true
    Url = "url-value"
    Supports = "supports-value"
}

Update-MgTeamworkWorkforceIntegration -WorkforceIntegrationId $workforceIntegrationId -BodyParameter $params

```