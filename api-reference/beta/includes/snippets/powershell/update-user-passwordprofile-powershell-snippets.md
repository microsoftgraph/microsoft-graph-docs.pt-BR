---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5560cf00ff42b60f3d1d8ee5a7730060a36a41b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118021"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    PasswordProfile = @{
        ForceChangePasswordNextSignIn = $false
        Password = "xWwvJ]6NMw+bWH-d"
    }
}

Update-MgUser -UserId $userId -BodyParameter $params

```