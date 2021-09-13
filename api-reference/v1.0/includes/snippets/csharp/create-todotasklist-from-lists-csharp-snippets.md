---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 577cd55f32c95cdf1d49e5b78433c592577254db0ea99df99ab9f87e4997c3f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = new TodoTaskList
{
    DisplayName = "Travel items"
};

await graphClient.Me.Todo.Lists
    .Request()
    .AddAsync(todoTaskList);

```