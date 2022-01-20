---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f4eea99fde05a8c3b1864f97fc86ba9cd172f5b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090417"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Email = "megan@contoso.com"
    IncludedSources = "mailbox, site"
}

New-MgComplianceEdiscoveryCaseCustodianUserSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```