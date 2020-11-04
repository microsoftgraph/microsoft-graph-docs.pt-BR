---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb7eb0fe17a609054ee02de41394b205c44c621f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = await graphClient.Me.Todo.Lists["AAMkADIyAAAAABrJAAA="]
    .Request()
    .GetAsync();

```