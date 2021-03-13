---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bfb826c3542fa9d9b7acaca2eed2059b0090586
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .Request()
    .DeleteAsync();

```