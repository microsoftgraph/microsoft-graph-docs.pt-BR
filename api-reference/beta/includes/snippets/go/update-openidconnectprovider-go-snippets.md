---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd86c46a1a6bca2ab4362c3ad7bbcb1aceee5f74
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323217"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProviderBase()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.socialIdentityProvider",
    "responseType": "id_token",
}
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Patch(requestBody)


```