---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2c45d2425b72f70c35996757445d1f2cf90cf7b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123063"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "football"
    )
    DisplayName = "Lyn Damer"
    WebUrl = "www.lyndamer.no"
}

New-MgUserProfileWebsite -UserId $userId -BodyParameter $params

```