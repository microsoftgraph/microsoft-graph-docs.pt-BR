---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54739431e009ca4e087b6fdd8db0645de139b949
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118820"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/alexd@contoso.com"
}

New-MgGroupRejectedSenderByRef -GroupId $groupId -BodyParameter $params

```