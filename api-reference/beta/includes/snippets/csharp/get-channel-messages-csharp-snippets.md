---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bac6ea6efca9ef93f3a94e6055f55adabdce3c0a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .GetAsync();

```