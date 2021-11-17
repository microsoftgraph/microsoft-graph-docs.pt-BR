---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb28ada3ad6592717faa94bed707fd6906928435
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015920"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MailFoldersRequestBuilderGetQueryParameters{
    IncludeHiddenFolders: true,
}
options := &msgraphsdk.MailFoldersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().MailFolders().Get(options)


```