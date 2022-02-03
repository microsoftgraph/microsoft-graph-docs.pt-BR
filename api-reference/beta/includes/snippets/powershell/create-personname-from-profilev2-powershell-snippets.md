---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 594de7a35e54b73aeb74cf32139c06b4297f05f2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350650"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Innocenty Popov"
    First = "Innocenty"
    Initials = "IP"
    Last = "Popov"
    LanguageTag = "en-US"
    Maiden = $null
}

# A UPN can also be used as -UserId.
New-MgUserProfileName -UserId $userId -BodyParameter $params

```