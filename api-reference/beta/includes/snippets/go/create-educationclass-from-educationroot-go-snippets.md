---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fda7b09d6c18bea042f11b1d6f713b95d51acc19
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083990"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
description := "Health Level 1"
requestBody.SetDescription(&description)
classCode := "Health 501"
requestBody.SetClassCode(&classCode)
displayName := "Health 1"
requestBody.SetDisplayName(&displayName)
externalId := "11019"
requestBody.SetExternalId(&externalId)
externalName := "Health Level 1"
requestBody.SetExternalName(&externalName)
externalSource := "sis"
requestBody.SetExternalSource(&externalSource)
mailNickname := "fineartschool.net"
requestBody.SetMailNickname(&mailNickname)
options := &msgraphsdk.ClassesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Classes().Post(options)


```