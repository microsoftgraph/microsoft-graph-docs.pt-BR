---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9799f0fa378f298a86b5a20610dee0ccba324623
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows
    .Request()
    .GetAsync();

```