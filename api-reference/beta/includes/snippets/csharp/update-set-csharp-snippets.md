---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e79f9b30d7cf9f15336cc43590ed288a7cf43c7
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = new Set
{
    Description = "mySet"
};

await graphClient.TermStore.Sets["{setId}"]
    .Request()
    .UpdateAsync(set);

```