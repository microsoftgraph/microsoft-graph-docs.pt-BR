---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a91d461497041fe12c744de808920f2707395887
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345845"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Key = "Base64-encoded-pfx-content"
    Password = "password-value"
}

Invoke-MgUploadTrustFrameworkKeySetPkcs12 -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```