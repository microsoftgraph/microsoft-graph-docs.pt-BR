---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e19d9af3d324fdbc234aabe19cb15b5421a9cd92
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{setId}"].Terms["{termId}"]
    .Request()
    .DeleteAsync();

```