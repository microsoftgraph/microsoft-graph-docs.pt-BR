---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b1ec0964254295e4d7ce476b16027f1c578b0f9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117371"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgGroupMemberByRef -GroupId $groupId -BodyParameter $params

```