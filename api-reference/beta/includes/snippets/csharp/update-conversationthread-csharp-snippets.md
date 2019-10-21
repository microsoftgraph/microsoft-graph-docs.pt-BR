---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7054feb5a7b1d1ddb6f2f2d401ef164cdfe7c150
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "35862865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    IsLocked = true
};

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .UpdateAsync(conversationThread);

```