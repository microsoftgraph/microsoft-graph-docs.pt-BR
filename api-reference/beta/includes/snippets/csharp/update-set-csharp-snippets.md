---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97984e5fca465954f84214a6ecdb147693fe0725
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = new Microsoft.Graph.TermStore.Set
{
    Description = "mySet"
};

await graphClient.TermStore.Sets["{termStore.set-id}"]
    .Request()
    .UpdateAsync(set);

```