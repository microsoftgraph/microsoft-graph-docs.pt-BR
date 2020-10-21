---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abbfb091f6ec6725e544267d46af2e1b06015d90
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .GetAsync();

```