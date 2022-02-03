---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d314465619efa6afaa6318d51fb5eaf05e7f6b73
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341782"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserTaskListTaskDelta -UserId $userId -BaseTaskListId $baseTaskListId

```