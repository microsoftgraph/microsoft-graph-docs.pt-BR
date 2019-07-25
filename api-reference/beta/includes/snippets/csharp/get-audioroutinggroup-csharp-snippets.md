---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ff0ac226b099411f11695298f95e7588bd862a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var AudioRoutingGroup = await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .GetAsync();

```