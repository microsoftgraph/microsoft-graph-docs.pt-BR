---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c108d33a6621f3fdcec71a62428e000e005b0f2a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTodoTask()
title := "A new task"
requestBody.SetTitle(&title)
requestBody.SetLinkedResources( []LinkedResource {
    msgraphsdk.NewLinkedResource(),
    SetAdditionalData(map[string]interface{}{
        "webUrl": "http://microsoft.com",
        "applicationName": "Microsoft",
        "displayName": "Microsoft",
    }
}
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Tasks().Post(options)


```