---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc08126d111b9d42fb0a396357cc10c8bbffa990
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = new Microsoft.Graph.TermStore.Set
{
    Description = "mySet"
};

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"]
    .Request()
    .UpdateAsync(set);

```