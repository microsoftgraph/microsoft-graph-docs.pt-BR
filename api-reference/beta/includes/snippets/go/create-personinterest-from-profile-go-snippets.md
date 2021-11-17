---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecb7ebde219a125749b7d78c2b55ecc71a30fe8d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980086"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
description := "World's greatest football club"
requestBody.SetDescription(&description)
displayName := "Chelsea FC"
requestBody.SetDisplayName(&displayName)
webUrl := "https://www.chelseafc.com"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.InterestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Interests().Post(options)


```