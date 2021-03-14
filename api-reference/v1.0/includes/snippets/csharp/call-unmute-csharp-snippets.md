---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04d96be82d47d31bf507390a98f8a1b9780374cd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```