---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f113d9760b05102278ca8adbc8ae865c96f1fe55
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .GetAsync();

```