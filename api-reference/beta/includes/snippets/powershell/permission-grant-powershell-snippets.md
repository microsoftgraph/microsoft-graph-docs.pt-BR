---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83155a50958f679c99fe5698dbd51db8304b3b4a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343051"
---
```powershell

Import-Module Microsoft.Graph.Files

$params = @{
    Recipients = @(
        @{
            Email = "john@contoso.com"
        }
        @{
            Email = "ryan@external.com"
        }
    )
    Roles = @(
        "read"
    )
}

Grant-MgSharePermission -SharedDriveItemId $sharedDriveItemId -BodyParameter $params

```