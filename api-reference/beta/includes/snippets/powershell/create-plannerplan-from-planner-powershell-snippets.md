---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61a2c961d4327dd1e77f3f2af3b5187a14c1b5cb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093882"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Container = @{
        Url = "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
    Title = "title-value"
}

New-MgPlannerPlan -BodyParameter $params

```