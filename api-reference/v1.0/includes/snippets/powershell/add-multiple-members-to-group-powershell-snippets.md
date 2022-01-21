---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd99020ea618975357d99cf5c0363a24ea126893
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117372"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "Members@odata.bind" = @(
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    )
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```