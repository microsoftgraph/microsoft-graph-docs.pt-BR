---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6eba6cd3ae67848b0a2d0b1727b25e7157af47d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .Request()
    .Expand("addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation")
    .GetAsync();

```