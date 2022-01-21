---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee530ca4a7ac095b22f69d031b938ac2c7a8348f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118018"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    CustomSecurityAttributes = @{
        Engineering = @{
            "@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
            ProjectDate = "2022-10-01"
        }
    }
}

Update-MgUser -UserId $userId -BodyParameter $params

```