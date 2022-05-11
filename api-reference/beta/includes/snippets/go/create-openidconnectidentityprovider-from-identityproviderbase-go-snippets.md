---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17e225c207dbf7c809f948a9c29cd8df32195b47
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProviderBase()
displayName := "Login with the Contoso identity provider"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid",
}
result, err := graphClient.Identity().IdentityProviders().Post(requestBody)


```