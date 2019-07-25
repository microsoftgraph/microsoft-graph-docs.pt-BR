---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1f77c5ea2102b0cc5ae408aa8f92dd05a4a1365
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```