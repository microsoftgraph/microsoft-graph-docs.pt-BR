---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e0637b63c0d8bf6132c5a98a303842df0e06177
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133584"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    EmailAddress = "kim@contoso.com"
}

New-MgUserAuthenticationEmailMethod -UserId $userId -BodyParameter $params

```