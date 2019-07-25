---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c5aca27fa617fe465b2eb63e14635906f807203
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```