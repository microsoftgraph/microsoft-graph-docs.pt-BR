---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8189b840b04b2651524a9eafb6495b56f1c336a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120901"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    ApplyHoldToSources = "false"
}

Update-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```