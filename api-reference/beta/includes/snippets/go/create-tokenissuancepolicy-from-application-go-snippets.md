---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03c7f1515862cb63c50c6e4b4d815084b858ca97
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410694"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
options := &msgraphsdk.TokenIssuancePolicyRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenIssuancePoliciesById(&tokenIssuancePolicyId).Post(options)


```