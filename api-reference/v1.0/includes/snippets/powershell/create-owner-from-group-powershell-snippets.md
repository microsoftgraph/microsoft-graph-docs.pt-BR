---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 152c77391214f07371b28c33618b7d5d2b66b1bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114788"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/{id}"
}

New-MgGroupOwnerByRef -GroupId $groupId -BodyParameter $params

```