---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a111be4745d63eb0ca93a85cf93811bfbdbcc5a7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411312"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/education/users/14011",
}
options := &msgraphsdk.EducationUserRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationUserId := "educationUser-id"
graphClient.Education().ClassesById(&educationClassId).TeachersById(&educationUserId).Post(options)


```