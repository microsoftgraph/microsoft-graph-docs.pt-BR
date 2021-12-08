---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0241b07667c2cce4630f042c94bfb665cde28e14
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347958"
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
options := &msgraphsdk.ConnectedOrganizationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizations().Post(options)


```