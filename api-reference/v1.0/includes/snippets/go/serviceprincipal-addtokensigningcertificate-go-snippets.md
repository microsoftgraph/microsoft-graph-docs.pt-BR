---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97a9aabe11cd85d558976dc2e501e99bc0bc8b36
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519215"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "CN=customDisplayName"
requestBody.SetDisplayName(&displayName)
endDateTime, err := time.Parse(time.RFC3339, "2024-01-25T00:00:00Z")
requestBody.SetEndDateTime(&endDateTime)
options := &msgraphsdk.AddTokenSigningCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AddTokenSigningCertificate().Post(options)


```