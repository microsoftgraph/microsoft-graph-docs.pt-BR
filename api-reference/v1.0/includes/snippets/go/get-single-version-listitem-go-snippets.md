---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c739c1c61a52839843279d83cef02d441febb94f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081779"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ListItemVersionRequestBuilderGetQueryParameters{
    Expand: "fields",
}
options := &msgraphsdk.ListItemVersionRequestBuilderGetOptions{
    Q: requestParameters,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
listItemVersionId := "listItemVersion-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).VersionsById(&listItemVersionId).Get(options)


```