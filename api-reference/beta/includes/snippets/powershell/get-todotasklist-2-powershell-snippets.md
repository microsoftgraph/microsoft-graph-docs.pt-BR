---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 985386020d94f4fb74f000dd92d19de1c7e4fb27
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350558"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```