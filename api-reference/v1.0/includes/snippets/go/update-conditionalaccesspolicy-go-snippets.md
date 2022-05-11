---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87749c9ab7cd706e11528a282e966aeed57af65a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConditionalAccessPolicy()
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
conditions.SetSignInRiskLevels( []RiskLevel {
    "high",
    "medium",
    "low",
}
conditionalAccessPolicyId := "conditionalAccessPolicy-id"
graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Patch(requestBody)


```