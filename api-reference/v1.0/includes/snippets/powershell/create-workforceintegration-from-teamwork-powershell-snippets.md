---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6789c7d4a5848d083c17f9d10bd1ba0c4f4ad28b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130231"
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
    SupportedEntities = "supportedEntities-value"
}

New-MgTeamworkWorkforceIntegration -BodyParameter $params

```