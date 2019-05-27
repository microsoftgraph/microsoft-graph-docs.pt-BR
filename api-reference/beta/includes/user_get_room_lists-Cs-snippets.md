---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b26c76d2aa31188f948665765326b3de612540dc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me.FindRoomLists()
    .Request()
    .GetAsync();

```