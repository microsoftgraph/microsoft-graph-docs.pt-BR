---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b81c390c250d4f1105535bdb7eb407bd70a1d030
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{id}"]
    .Request()
    .GetAsync();

```