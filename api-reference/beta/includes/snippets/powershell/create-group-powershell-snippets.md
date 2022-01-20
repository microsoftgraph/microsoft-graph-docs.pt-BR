---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 605086f4f718accb5d7753501c9bc293e8576490
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127710"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Self help community for golf"
    DisplayName = "Golf Assist"
    GroupTypes = @(
        "Unified"
    )
    MailEnabled = $true
    MailNickname = "golfassist"
    SecurityEnabled = $false
}

New-MgGroup -BodyParameter $params

```