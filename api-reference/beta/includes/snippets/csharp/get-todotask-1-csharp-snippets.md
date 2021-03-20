---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc487eac61786fafab2b83e3ad8b919fa268ab69
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .GetAsync();

```