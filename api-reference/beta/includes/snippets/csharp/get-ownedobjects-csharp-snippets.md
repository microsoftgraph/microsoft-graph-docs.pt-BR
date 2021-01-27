---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31fbac4832f3ebacf87ec9113eb10ca3a93dabdf
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.ServicePrincipals["{id}"].OwnedObjects
    .Request()
    .GetAsync();

```