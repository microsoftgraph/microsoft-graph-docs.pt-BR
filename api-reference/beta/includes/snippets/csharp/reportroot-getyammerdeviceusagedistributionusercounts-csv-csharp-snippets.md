---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c014f92fbaa82800d73e3c719e25d03f142ce163
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetYammerDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```