---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31a56258c6964991777e226a89c67118eee244bc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
};

await graphClient.RiskyUsers
    .Dismiss(userIds)
    .Request()
    .PostAsync();

```