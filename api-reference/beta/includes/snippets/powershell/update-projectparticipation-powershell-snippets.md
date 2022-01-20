---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51905f03d3bbfb4dffb58377470e2e87872aea03
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112079"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
    Client = @{
        Department = "Corporate Marketing"
        WebUrl = "https://www.contoso.com"
    }
}

Update-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId -BodyParameter $params

```