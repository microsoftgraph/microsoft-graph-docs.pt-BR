---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e184ad03946dd2df75f42a9c4b8876204b1b065d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322576"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
accessReviewStageId := "accessReviewStage-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).StagesById(&accessReviewStageId).Stop(accessReviewScheduleDefinition-id, accessReviewInstance-id, accessReviewStage-id).Post()


```