---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06e66b6735723e715cff17cb237ea8c6ea3d5715efdbfb09ed55e7bc0e156b35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var estimateStatisticsOperation = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].LastEstimateStatisticsOperation
    .Request()
    .GetAsync();

```