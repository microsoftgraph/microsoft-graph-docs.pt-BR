---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a94b31f4799730cd2c12480606f4af4daa9130ea
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myDecisions = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].MyDecisions
    .Request()
    .GetAsync();

```