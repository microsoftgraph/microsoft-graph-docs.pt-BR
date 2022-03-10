---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef12167a60b35f4cb9c9b1a28441c417e31f4d5a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}",
    "@odata.type": "#microsoft.graph.identityProvider",
}
options := &msgraphsdk.IdentityProviderBaseRequestBuilderPatchOptions{
    Body: requestBody,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserFlowIdentityProvidersById(&identityProviderBaseId).Patch(options)


```