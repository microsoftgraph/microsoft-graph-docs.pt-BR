---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7380de569df1d4e5c377aa413cf7525dae516d65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349801"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    CountryCode = "NO"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId -BodyParameter $params

```