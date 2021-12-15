---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe3d5408450ab84889057e0404e52e0169e94e3d
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Tasks.Lists.AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=.Tasks.Delta
    .Request()
    .GetAsync();

```