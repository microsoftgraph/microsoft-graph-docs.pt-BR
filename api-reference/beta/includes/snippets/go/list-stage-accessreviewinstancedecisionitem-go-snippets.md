---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bfb71e8ae9a07c7216f6056771c50bc544fc91d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322577"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
accessReviewStageId := "accessReviewStage-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).StagesById(&accessReviewStageId).Decisions().Get()


```