---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13d69936df854c83020affc84ccdcf40fdb4734a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "directories":  []Object {
    }
    "synchronizationRules":  []Object {
    }
}
options := &msgraphsdk.SchemaRequestBuilderPutOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Schema().Put(options)


```