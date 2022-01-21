---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97a8dc5cf4888b6204a7fe909e937971ee2f5a00
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132786"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Branding"
    )
    Client = @{
        DisplayName = "Contoso Ltd."
        Department = "Corporate Marketing"
        WebUrl = "https://www.contoso.com"
    }
    DisplayName = "Contoso Re-branding Project"
    Detail = @{
        Company = @{
            DisplayName = "Adventureworks Inc."
            Department = "Consulting"
            WebUrl = "https://adventureworks.com"
        }
        Description = "Rebranding of Contoso Ltd."
        JobTitle = "Lead PM Rebranding"
        Role = "project management"
        Summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
    }
}

New-MgUserProfileProject -UserId $userId -BodyParameter $params

```