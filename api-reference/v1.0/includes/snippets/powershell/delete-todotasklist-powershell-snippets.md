---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9584e934ec819311cd0b83c1abb4710a8e5dcac8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349368"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Remove-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```