---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27b76a80fdb94160d34cee665325866b9423f817
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125401"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
appId := "65415bb1-9267-4313-bbf5-ae259732ee12"
requestBody.SetAppId(&appId)
options := &msgraphsdk.ServicePrincipalsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.ServicePrincipals().Post(options)


```