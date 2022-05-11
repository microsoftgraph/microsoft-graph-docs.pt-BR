---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d96b253d353cf661d585f6fe1ef91018de206f8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325623"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationMethodConfiguration()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "allowExternalIdToUseEmailOtp": "disabled",
}
authenticationMethodConfigurationId := "authenticationMethodConfiguration-id"
graphClient.Policies().AuthenticationMethodsPolicy().AuthenticationMethodConfigurationsById(&authenticationMethodConfigurationId).Patch(requestBody)


```