---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a51a9b01e32a65045c50b113812b8837f537393
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202867"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewParametersRequestBody()
requestBody.SetParameters( []SynchronizationJobApplicationParameters {
    msgraphsdk.NewSynchronizationJobApplicationParameters(),
    SetAdditionalData(map[string]interface{}{
        "subjects":  []Object {
        }
        "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca",
    }
}
options := &msgraphsdk.ProvisionOnDemandRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).ProvisionOnDemand(servicePrincipal-id, synchronizationJob-id).Post(options)


```