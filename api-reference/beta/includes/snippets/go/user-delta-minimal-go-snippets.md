---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cfb9616e9f108ed5e880b100669d18aef8b3010
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.UserRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Get(options)


```