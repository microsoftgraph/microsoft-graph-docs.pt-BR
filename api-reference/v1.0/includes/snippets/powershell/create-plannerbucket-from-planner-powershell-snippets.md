---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c937afd98b7aff2a5c24dab443797546fc9a0447
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132309"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Name = "Advertising"
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    OrderHint = " !"
}

New-MgPlannerBucket -BodyParameter $params

```