---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9229374808fa4cbb9c1bf60ac12478a3cfa934b2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115546"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AdditionalInformation = "additionalInformation-after-update"
    Confidence = 42
    Description = "description-after-update"
}

Update-MgSecurityTiIndicator -TiIndicatorId $tiIndicatorId -BodyParameter $params

```