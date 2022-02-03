---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4485b6f52e0ba95463487fec900e2ed1ec63fb70
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346152"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisableUserAccounts = $true
}

Invoke-MgForceDomainDelete -DomainId $domainId -BodyParameter $params

```