---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47acff6372d0783f51b0f1f45277837559fd334a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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