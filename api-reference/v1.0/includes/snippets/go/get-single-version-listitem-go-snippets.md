---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e3513b4e9d239a3313bdc1a30a0ed89bd217737
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033211"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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