---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad2dcfdd60a91ed11b52fefdea09b8fe3ecfc143
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137457"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Users().Delta()().Get(options)


```