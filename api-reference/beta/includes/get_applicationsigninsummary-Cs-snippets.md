---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9143c487bfa18897525ea7139e65df44ae584d4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports.GetAzureADApplicationSignInSummary('D7')
    .Request()
    .GetAsync();

```