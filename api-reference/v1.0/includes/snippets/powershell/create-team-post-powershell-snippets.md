---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de3ce27edd358e2d4b7f3542e52d1f8f098f7d7f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087684"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
    DisplayName = "My Sample Team"
    Description = "My Sample Team’s Description"
}

New-MgTeam -BodyParameter $params

```