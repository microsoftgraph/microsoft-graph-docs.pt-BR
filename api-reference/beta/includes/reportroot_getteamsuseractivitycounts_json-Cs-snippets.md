---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53bb91fe6b0ef4c7f2690e7879063bc040a37117
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityCounts = await graphClient.Reports.GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```