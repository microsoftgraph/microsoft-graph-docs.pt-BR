---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8990889742c7245fe14cd0826e14aae458afab29
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083239"
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
options := &msgraphsdk.B2xUserFlowsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().B2xUserFlows().Post(options)


```