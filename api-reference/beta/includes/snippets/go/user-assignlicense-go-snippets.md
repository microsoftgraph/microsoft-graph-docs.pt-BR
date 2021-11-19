---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6dede37136ae81665c734969fc4ba15c0b3b327
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085955"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
        }
        "skuId": "skuId-value-1",
    }
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235",
        }
        "skuId": "skuId-value-2",
    }
}
requestBody.SetRemoveLicenses( []string {
}
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().AssignLicense().Post(options)


```