---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 180565d789f55f1ab91ef2eb47ccde49ffe4f578
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322979"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
decision := "Approve"
requestBody.SetDecision(&decision)
justification := "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team"
requestBody.SetJustification(&justification)
resourceId := "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
requestBody.SetResourceId(&resourceId)
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).BatchRecordDecisions(accessReviewScheduleDefinition-id, accessReviewInstance-id).Post(requestBody)


```