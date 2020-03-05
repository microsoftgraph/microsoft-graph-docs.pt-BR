---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1d9a2b3b29c7b0a46a033c2cc922c1cd11594d6
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies["homeRealmDiscoveryPolicies"].{id}
    .Request()
    .DeleteAsync();

```