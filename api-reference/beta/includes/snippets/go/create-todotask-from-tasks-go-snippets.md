---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8def01969d0e8d809ee2c768cd00d4f637581041
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098648"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTask()
title := "A new task"
requestBody.SetTitle(&title)
requestBody.SetCategories( []String {
    "Important",
}
requestBody.SetLinkedResources( []LinkedResource {
    msgraphsdk.NewLinkedResource(),
webUrl := "http://microsoft.com"
    SetWebUrl(&webUrl)
applicationName := "Microsoft"
    SetApplicationName(&applicationName)
displayName := "Microsoft"
    SetDisplayName(&displayName)
}
todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Tasks().Post(requestBody)


```