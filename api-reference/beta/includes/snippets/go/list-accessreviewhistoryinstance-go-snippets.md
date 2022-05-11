---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 990e080a99578b475b4f43137bb029706623f900
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322617"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewHistoryDefinitionId := "accessReviewHistoryDefinition-id"
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById(&accessReviewHistoryDefinitionId).Instances().Get()


```