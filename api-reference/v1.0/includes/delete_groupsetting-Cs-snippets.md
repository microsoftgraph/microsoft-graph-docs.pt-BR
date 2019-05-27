---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac7a5220305ade46784fe47cf9ca27499b8a93b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{id}"]
    .Request()
    .DeleteAsync();

```