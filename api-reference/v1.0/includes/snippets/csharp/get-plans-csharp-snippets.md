---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 434034643c030934071ee58a185954fed0efce7d
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015621"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Planner.Plans
    .Request()
    .GetAsync();

```