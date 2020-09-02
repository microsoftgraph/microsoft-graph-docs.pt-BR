---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a924f2ed95760c4de19362a8a1fd47a24b04000c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = await graphClient.Identity.B2xUserFlows["{id}"]
    .Request()
    .GetAsync();

```