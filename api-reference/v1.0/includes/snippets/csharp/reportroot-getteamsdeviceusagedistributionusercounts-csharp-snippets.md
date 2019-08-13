---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 441546c9d3508201deaa97396ed4fcc6f25120a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```