---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a53abb0fb13c45e9efe8eb9b80a6a8d37267aa4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127452"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId

```