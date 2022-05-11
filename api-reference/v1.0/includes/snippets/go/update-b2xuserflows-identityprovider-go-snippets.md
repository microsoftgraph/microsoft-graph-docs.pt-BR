---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17434c73c49feb0e8d8c27f90659961707dfb3cb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH",
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityProviderId := "identityProvider-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).IdentityProvidersById(&identityProviderId).Post(requestBody)


```