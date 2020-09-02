---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f79632839aee4de1b1137e85045ec8150efb6f39
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows
    .Request()
    .Expand("identityProviders")
    .GetAsync();

```