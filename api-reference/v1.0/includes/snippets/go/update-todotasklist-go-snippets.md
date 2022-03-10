---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ae64ae0924d82dfca680884c917741bafb53fc1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Vacation Plan"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.TodoTaskListRequestBuilderPatchOptions{
    Body: requestBody,
}
todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Patch(options)


```