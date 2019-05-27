---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e79ea48acdd97930128a36235dd995841e3370cb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityMinuteCounts = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```