---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 309e21da8b4aa11410d504f5d0c702c8a2c4f39f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```