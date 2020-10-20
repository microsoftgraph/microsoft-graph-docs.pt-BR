---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35f5686cb351b5181c30b5d633b84e3c12404e74
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Unsubscribe()
    .Request()
    .PostAsync();

```