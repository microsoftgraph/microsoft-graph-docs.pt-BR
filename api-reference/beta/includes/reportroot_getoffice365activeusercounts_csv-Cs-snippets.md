---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9339918ea5335ba43acad5af7121c15603be954d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserCounts = await graphClient.Reports.GetOffice365ActiveUserCounts('D7')
    .Request()
    .GetAsync();

```