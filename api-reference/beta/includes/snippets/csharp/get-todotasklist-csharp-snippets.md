---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb7eb0fe17a609054ee02de41394b205c44c621f
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = await graphClient.Me.Todo.Lists["AAMkADIyAAAAABrJAAA="]
    .Request()
    .GetAsync();

```