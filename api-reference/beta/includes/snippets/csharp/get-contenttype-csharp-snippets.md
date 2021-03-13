---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79470a20ca68eebc733d4905d8644e4db9b4e4e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Request()
    .GetAsync();

```