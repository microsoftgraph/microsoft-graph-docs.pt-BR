---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf863cc601f5c0860381c6110e5cf95da81c84e6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115782"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgServicePrincipalOwnerByRef -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```