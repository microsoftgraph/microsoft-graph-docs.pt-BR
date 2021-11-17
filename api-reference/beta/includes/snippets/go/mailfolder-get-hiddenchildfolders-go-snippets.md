---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4458a4858b1f19686e0f390ed5fb8bbc8c8fceea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018532"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChildFoldersRequestBuilderGetQueryParameters{
    IncludeHiddenFolders: true,
}
options := &msgraphsdk.ChildFoldersRequestBuilderGetOptions{
    Q: requestParameters,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Get(options)


```