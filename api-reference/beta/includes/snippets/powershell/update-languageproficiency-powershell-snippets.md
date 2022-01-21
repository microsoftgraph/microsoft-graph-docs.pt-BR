---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a080635f441aba8fc78d7fd06427974bce4e3ab0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116147"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
}

Update-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId -BodyParameter $params

```