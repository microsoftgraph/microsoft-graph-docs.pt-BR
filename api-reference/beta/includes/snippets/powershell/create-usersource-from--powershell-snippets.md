---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a7cf2f0ebd7250ebc97115b0361dccc154ec462
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438643"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Email = "admin@M365x809305.onmicrosoft.com"
    IncludedSources = "mailbox, site"
}

New-MgSecurityCaseEdiscoveryCaseLegalHoldUserSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryHoldPolicyId $ediscoveryHoldPolicyId -BodyParameter $params

```