---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26b72e4a7ce9b9843def0f31363570d5579acf7b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Planner.All.Delta()
    .Request()
    .GetAsync();

```