---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a1b60d3211d0eb3ba203c718addf3514de6addd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133149"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Name = "Development"
}

Update-MgPlannerBucket -PlannerBucketId $plannerBucketId -BodyParameter $params

```