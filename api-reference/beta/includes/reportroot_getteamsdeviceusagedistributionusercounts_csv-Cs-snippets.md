---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1db9e01b2d37f5398269bd7dfc47cd0d7773704f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageDistributionUserCounts = await graphClient.Reports.GetTeamsDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```