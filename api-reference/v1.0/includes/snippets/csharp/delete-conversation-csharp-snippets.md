---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a04d006b19ff7bbac1e73c7c6dc22aeb8c1c772
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605243"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Conversations["{id}"]
    .Request()
    .DeleteAsync();

```