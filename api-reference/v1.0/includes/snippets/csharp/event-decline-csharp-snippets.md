---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd49d5e09242ead3a138a58f66b4896e77edd605
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Decline(null,sendResponse,comment)
    .Request()
    .PostAsync();

```