---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac3e003371010cd4e57b9d23bf6391230e435d62
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784080"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["{message-id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```