---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28f6211dfa841ad3ef85abc23f119b4bd2163726
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125421"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    AppRoleAssignmentRequired = $true
}

Update-MgServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```