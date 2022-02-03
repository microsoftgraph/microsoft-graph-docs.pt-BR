---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 300da59440515aeded59b3682834aa26f8ae3007
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348605"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PasswordCredential = @{
        DisplayName = "Password friendly name"
    }
}

Add-MgServicePrincipalPassword -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```