---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7ec8819005c21715473378fe105484d3c0f26e6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var people = await graphClient.Me.People
    .Request()
    .GetAsync();

```