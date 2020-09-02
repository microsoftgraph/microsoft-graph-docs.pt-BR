---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aee4d1862f45ee2da5c1a6c765d5574739f44f6c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.TermStore.Sets["{setId}"]
    .Request()
    .GetAsync();

```