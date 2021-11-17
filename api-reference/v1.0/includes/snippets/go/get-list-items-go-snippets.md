---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45b453c26752f14ad636fb59c110eddbed90ff76
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004055"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ItemsRequestBuilderGetQueryParameters{
    Expand: "fields(select=Name,Color,Quantity)",
}
options := &msgraphsdk.ItemsRequestBuilderGetOptions{
    Q: requestParameters,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Items().Get(options)


```