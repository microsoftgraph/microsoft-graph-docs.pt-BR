---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 141f966b551e1cc9c821c73b525fdbb423b2fb08
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroups = await graphClient.App.Calls["{id}"].AudioRoutingGroups
    .Request()
    .GetAsync();

```