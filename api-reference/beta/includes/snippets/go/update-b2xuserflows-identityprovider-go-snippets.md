---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2245de3e8d518cb543e1fb5b9f5188fc028801ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990804"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).IdentityProviders().$ref().Post(options)


```