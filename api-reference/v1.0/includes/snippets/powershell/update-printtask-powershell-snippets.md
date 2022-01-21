---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b198973e309a055577626d1cf5beb3bef6ce18e2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088267"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    Status = @{
        State = "completed"
        Description = "completed"
    }
}

Update-MgPrintTaskDefinitionTask -PrintTaskDefinitionId $printTaskDefinitionId -PrintTaskId $printTaskId -BodyParameter $params

```