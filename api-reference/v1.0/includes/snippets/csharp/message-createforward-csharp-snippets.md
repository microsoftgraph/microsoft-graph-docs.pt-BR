---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7272e6d75c7296e681936022e2f7f9c9921822b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateForward(null,null,null)
    .Request()
    .PostAsync();

```