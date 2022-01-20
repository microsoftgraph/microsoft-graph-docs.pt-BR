---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75125428c0b191b836a7f9887819db36262dcb5a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123896"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Site = @{
        WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
    }
}

New-MgComplianceEdiscoveryCaseLegalHoldSiteSource -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```