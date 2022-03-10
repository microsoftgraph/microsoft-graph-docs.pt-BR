---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a60c62967c3795c5edcb38555fe49665ab8a167d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410789"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/{userId}",
}
options := &msgraphsdk.UserRequestBuilderPostOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
userId := "user-id"
graphClient.Print().SharesById(&printerShareId).AllowedUsersById(&userId).Post(options)


```