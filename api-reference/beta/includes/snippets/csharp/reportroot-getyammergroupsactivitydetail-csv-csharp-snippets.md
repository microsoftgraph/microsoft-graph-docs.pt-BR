---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 535fee916ada5536004bf53b4bd11500d10b30b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityDetail = await graphClient.Reports
    .GetYammerGroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```