---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 385771c515d86f15f1ddc3900961b209ee67fc49
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351597"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolder -UserId $userId -Includehiddenfolders true 

```