---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1df4d26b114dace6d6fe62743da23389fdd9db05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325501"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).DecisionsById(&accessReviewInstanceDecisionItemId).Get()


```