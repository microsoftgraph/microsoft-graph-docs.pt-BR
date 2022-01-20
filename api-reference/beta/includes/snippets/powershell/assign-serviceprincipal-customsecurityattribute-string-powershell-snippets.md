---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2e4511a52893024062c309d7107e9c63e2acb8f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125422"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    CustomSecurityAttributes = @{
        Engineering = @{
            "@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
            ProjectDate = "2022-10-01"
        }
    }
}

Update-MgServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```