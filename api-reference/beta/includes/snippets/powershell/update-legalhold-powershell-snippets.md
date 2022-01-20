---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbe9809ab2efa67ce7659974276fc7b2aabf1d71
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090396"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Description = "This is a description for a legalHold"
}

Update-MgComplianceEdiscoveryCaseLegalHold -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```