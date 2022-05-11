---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83d60e29aff0badab13318a7523e22724e5f4091
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324719"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2xIdentityUserFlow()
id := "UserFlowWithAPIConnector"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(1)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
apiConnectorConfiguration := msgraphsdk.NewUserFlowApiConnectorConfiguration()
requestBody.SetApiConnectorConfiguration(apiConnectorConfiguration)
postFederationSignup := msgraphsdk.NewIdentityApiConnector()
apiConnectorConfiguration.SetPostFederationSignup(postFederationSignup)
postFederationSignup.SetAdditionalData(map[string]interface{}{
    "@odata.id": "{apiConnectorId}",
}
postAttributeCollection := msgraphsdk.NewIdentityApiConnector()
apiConnectorConfiguration.SetPostAttributeCollection(postAttributeCollection)
postAttributeCollection.SetAdditionalData(map[string]interface{}{
    "@odata.id": "{apiConnectorId}",
}
result, err := graphClient.Identity().B2xUserFlows().Post(requestBody)


```