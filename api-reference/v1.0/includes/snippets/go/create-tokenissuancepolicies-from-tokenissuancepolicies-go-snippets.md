---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9eedf8698b57c9f2c0f39807f8aefb7f95134736
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095236"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTokenIssuancePolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.TokenIssuancePoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().TokenIssuancePolicies().Post(options)


```