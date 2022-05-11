---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79e103ee60bcf9b376061c4e100bce7ffcfecdc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324674"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProviderBase()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.socialIdentityProvider",
    "clientSecret": "1111111111111",
}
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Patch(requestBody)


```