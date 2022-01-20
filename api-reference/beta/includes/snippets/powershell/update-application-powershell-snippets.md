---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b41607451390d7d3470f2078b916802cbf3b8fac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126170"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "New display name"
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```