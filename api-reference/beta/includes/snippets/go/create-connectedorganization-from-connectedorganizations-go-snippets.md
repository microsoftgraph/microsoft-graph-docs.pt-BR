---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6904737dc8c94de7a412cbebebbdc600fe5d57b0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConnectedOrganization()
displayName := "Connected organization name"
requestBody.SetDisplayName(&displayName)
description := "Connected organization description"
requestBody.SetDescription(&description)
requestBody.SetIdentitySources( []IdentitySource {
    msgraphsdk.NewIdentitySource(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.domainIdentitySource",
        "domainName": "example.com",
        "displayName": "example.com",
    }
}
state := "proposed"
requestBody.SetState(&state)
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizations().Post(requestBody)


```