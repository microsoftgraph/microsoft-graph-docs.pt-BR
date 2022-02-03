---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28a18f7a4259212b968dbc57122dd2538fccd488
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350725"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    WebUrl = "https://github.com/innocenty.popov"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId -BodyParameter $params

```