---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 019425ff86e2b172c692fd8efd6c84b937dcea82
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterOperators = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema.FilterOperators()
    .Request()
    .GetAsync();

```