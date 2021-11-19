---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0278ba08a08a3e14dce251cc37575573d2762754
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityApiConnector()
authenticationConfiguration := msgraphsdk.NewApiAuthenticationConfigurationBase()
requestBody.SetAuthenticationConfiguration(authenticationConfiguration)
authenticationConfiguration.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret",
}
options := &msgraphsdk.IdentityApiConnectorRequestBuilderPatchOptions{
    Body: requestBody,
}
identityApiConnectorId := "identityApiConnector-id"
graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Patch(options)


```