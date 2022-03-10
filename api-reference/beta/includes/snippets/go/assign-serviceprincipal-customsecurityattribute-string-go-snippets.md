---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7d251dc714cf18b97e188cf0950a8cd040ca50b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411570"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
customSecurityAttributes := msgraphsdk.NewCustomSecurityAttributeValue()
requestBody.SetCustomSecurityAttributes(customSecurityAttributes)
customSecurityAttributes.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.ServicePrincipalRequestBuilderPatchOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Patch(options)


```