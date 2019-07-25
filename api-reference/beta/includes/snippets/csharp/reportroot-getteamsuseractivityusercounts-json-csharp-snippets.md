---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d06f971539fa5c73f5561d2d025a64c2ac41edc4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserCounts = await graphClient.Reports
    .GetTeamsUserActivityUserCounts('D7')
    .Request()
    .GetAsync();

```