---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e0fcfe34ab96dbf8fdf03059a1ccfc82405fdbd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133535"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Contoso Life v2.0"
    DisplayName = "Contoso Life Renewed"
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```