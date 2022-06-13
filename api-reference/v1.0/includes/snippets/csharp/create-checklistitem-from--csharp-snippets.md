---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18ad4517bb2616d698da9a60f2bd3b85c3115fcc
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66041014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var checklistItem = new ChecklistItem
{
    DisplayName = "Final sign-off from the team"
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].ChecklistItems
    .Request()
    .AddAsync(checklistItem);

```