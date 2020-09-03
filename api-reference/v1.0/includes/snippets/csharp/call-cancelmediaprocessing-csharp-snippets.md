---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11dbab6d04a2f95e8117a5fe425deda9b0fd6238
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{id}"]
    .CancelMediaProcessing(clientContext)
    .Request()
    .PostAsync();

```