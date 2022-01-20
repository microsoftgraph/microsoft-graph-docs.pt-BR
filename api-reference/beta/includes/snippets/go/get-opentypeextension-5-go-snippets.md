---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 690f0921dbc6ddfe6d8b26f022a48594734295b7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Filter: "Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')",
    Expand: "Extensions($filter=id%20eq%20'Com.Contoso.Referral')",
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Messages().Get(options)


```