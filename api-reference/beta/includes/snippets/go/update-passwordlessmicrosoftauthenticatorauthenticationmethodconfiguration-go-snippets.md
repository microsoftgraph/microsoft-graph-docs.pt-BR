---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea3f709b9def50366c12b1062176702969902735
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395402"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationMethodConfiguration()
state := "enabled"
requestBody.SetState(&state)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
}
options := &msgraphsdk.AuthenticationMethodConfigurationRequestBuilderPatchOptions{
    Body: requestBody,
}
authenticationMethodConfigurationId := "authenticationMethodConfiguration-id"
result, err := graphClient.Policies().AuthenticationMethodsPolicy().AuthenticationMethodConfigurationsById(&authenticationMethodConfigurationId).Patch(options)


```