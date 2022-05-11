---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38fbfee595cd2497695e290af3892e8afba9a39f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).TokenLifetimePolicies().Post(requestBody)


```