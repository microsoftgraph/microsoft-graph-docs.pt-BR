---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0701b403c37efde672695bba06bb9ec958adf8ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = new TodoTaskList
{
    DisplayName = "Vacation Plan"
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .UpdateAsync(todoTaskList);

```