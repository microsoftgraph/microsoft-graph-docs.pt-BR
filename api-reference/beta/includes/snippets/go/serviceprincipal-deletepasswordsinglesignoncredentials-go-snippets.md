---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d34a11f5719045f3104f2bac718298b824fcf498
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410597"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdRequestBody()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
options := &msgraphsdk.DeletePasswordSingleSignOnCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).DeletePasswordSingleSignOnCredentials(servicePrincipal-id).Post(options)


```