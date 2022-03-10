---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8275c59099dd5efbf02d1746fee5e467ee07c69a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411525"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnotation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.PersonAnnotationRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
personAnnotationId := "personAnnotation-id"
result, err := graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Patch(options)


```