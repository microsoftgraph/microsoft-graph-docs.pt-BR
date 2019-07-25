---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 186edfed09c4d5856ad16a303ea42e1cc2ed8432
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872680"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageDetail = await graphClient.Reports
    .GetSharePointSiteUsageDetail('D7')
    .Request()
    .GetAsync();

```