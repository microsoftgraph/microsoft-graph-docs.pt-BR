---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a33142c3c43189756fe2c383c8ce64d9923daded
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438792"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    DisplayName = "CONTOSO LITIGATION-005"
    Description = "Project Bazooka"
    ExternalId = "324516"
}

New-MgSecurityCaseEdiscoveryCase -BodyParameter $params

```