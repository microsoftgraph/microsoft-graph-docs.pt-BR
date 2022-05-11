---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32515a9c99bc7da3132a15223be6323870d69924
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322909"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}",
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityProviderId := "identityProvider-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).IdentityProvidersById(&identityProviderId).Post(requestBody)


```