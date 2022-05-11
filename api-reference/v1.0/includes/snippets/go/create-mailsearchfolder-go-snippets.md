---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aaee37a4abcdcb9e6aa97173d86ab1bab34e9611
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325196"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "Weekly digests"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.mailSearchFolder",
    "includeNestedFolders": true,
    "sourceFolderIds":  []String {
        "AQMkADYAAAIBDAAAAA==",
    }
    "filterQuery": "contains(subject, 'weekly digest')",
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Post(requestBody)


```