---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21ab5b4454c31f3299eb676dfbfe6d96c066309b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["socketIo"]
    .Request()
    .GetAsync();

```