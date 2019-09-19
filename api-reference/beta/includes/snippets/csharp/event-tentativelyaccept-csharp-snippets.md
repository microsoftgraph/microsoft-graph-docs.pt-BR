---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be522034fc6c17a23df04492630a61f75290b82e
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37045306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .TentativelyAccept(sendResponse,comment)
    .Request()
    .PostAsync();

```