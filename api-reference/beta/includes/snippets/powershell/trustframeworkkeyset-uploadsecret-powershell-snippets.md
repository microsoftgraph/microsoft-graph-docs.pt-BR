---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b8fb8032331627f0f72abb10b4737a023522d3f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346395"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Use = "use-value"
    K = "application-secret-to-be-uploaded"
    Nbf = 1508969811
    Exp = 1508973711
}

Invoke-MgUploadTrustFrameworkKeySetSecret -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```