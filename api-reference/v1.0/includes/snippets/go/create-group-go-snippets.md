---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 477987af6e2fd012436825a771a287b82da660d7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroup()
description := "Self help community for library"
requestBody.SetDescription(&description)
displayName := "Library Assist"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []String {
    "Unified",
}
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled)
mailNickname := "library"
requestBody.SetMailNickname(&mailNickname)
securityEnabled := false
requestBody.SetSecurityEnabled(&securityEnabled)
options := &msgraphsdk.GroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Groups().Post(options)


```