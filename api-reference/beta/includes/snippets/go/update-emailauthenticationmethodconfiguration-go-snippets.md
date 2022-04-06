---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4bb9506c5801c61ef65753e59498b875a7c78cd
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528045"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationMethodConfiguration()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "allowExternalIdToUseEmailOtp": "disabled",
}
options := &msgraphsdk.AuthenticationMethodConfigurationRequestBuilderPatchOptions{
    Body: requestBody,
}
authenticationMethodConfigurationId := "authenticationMethodConfiguration-id"
graphClient.Policies().AuthenticationMethodsPolicy().AuthenticationMethodConfigurationsById(&authenticationMethodConfigurationId).Patch(options)


```