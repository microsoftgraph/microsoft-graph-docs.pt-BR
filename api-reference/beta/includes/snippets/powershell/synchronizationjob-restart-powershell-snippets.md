---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f20a78315399f74ec15d8edb1be045eba0e930a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349073"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Criteria = @{
        ResetScope = "Watermark, Escrows, QuarantineState"
    }
}

Restart-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```