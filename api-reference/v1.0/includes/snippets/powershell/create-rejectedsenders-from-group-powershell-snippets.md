---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cf80af7c2cba7053f00a7e0c914fa21d62e7963
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117329"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}

New-MgGroupRejectedSenderByRef -GroupId $groupId -BodyParameter $params

```