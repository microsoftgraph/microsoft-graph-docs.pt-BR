---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec0d5afcae728bb6f39d26926de04af9ee23b6f2
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{id}"].Members.Microsoft.graph.user.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```