---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54ce2112ea02055c4585091a90e535251369a501
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410848"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewKeyIdRequestBody()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
options := &msgraphsdk.RemovePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).RemovePassword(servicePrincipal-id).Post(options)


```