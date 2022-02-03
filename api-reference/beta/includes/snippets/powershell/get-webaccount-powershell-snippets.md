---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53fbbf1726ccf7bb2e2fc2254b964e264be8e119
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349328"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId

```