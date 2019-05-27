---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4749c2ac9827b238b7827558057fe468f721d3f9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```