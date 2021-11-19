---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7eb39fb2d8ff0442c9b71379ca34dbf0e6de11f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095237"
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
graphClient.Me().Todo().ListsById(&todoTaskListId).Patch(options)


```