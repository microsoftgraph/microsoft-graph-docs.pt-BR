---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddffc8e2a6c9b51a72b2c30076fe21bf2a575d24
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Devices["{device-id}"].TransitiveMemberOf
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName, 'a')")
    .OrderBy("displayName")
    .GetAsync();

```