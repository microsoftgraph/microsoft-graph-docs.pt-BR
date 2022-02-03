---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03839de623dc25f7def75393a04a3ba816921c3a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344513"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Use = "sig"
    Kty = "RSA"
    Nbf = 1508969811
    Exp = 1508969811
}

New-MgTrustFrameworkKeySetKey -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```