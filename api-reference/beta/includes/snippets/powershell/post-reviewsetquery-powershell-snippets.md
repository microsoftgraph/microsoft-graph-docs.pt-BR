---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23e84b52de95f235119af52cb5a5a76a09891fed
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090375"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Query 1"
    Query = "(subject:"Quarterly Financials")"
}

New-MgComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```