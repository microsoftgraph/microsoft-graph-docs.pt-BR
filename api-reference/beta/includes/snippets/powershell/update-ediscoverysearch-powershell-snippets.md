---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a690750a02d96558dd7a59ddac5adbc97f2ca575
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446642"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    DisplayName = "Teams search"
}

Update-MgSecurityCaseEdiscoveryCaseSearch -EdiscoveryCaseId $ediscoveryCaseId -EdiscoverySearchId $ediscoverySearchId -BodyParameter $params

```