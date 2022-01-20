---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2c28517d8d866ee5e4b53a6c560800c004be207
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110287"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    BusinessPhones = @(
        "+1 425 555 0109"
    )
    OfficeLocation = "18/2111"
}

Update-MgUser -UserId $userId -BodyParameter $params

```