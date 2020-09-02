---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31b65800dc38bbd5853ca40c150f1e1154f195ca
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{id}"]
    .Request()
    .DeleteAsync();

```