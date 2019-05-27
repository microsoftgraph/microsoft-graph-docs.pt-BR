---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf0702b42e4988f7e3d5b7becdcc34414be17de5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers["006111db-0810-4494-a6df-904d368bd81b"]
    .Request()
    .DeleteAsync();

```