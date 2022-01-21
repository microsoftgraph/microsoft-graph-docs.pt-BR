---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31020ecc5f4e784b5182c4f7453c588567ce78c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088688"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Name = "Contoso HR Service Tickets"
    Description = "Connection to index HR service tickets"
}

Update-MgExternalConnection -ExternalConnectionId $externalConnectionId -BodyParameter $params

```