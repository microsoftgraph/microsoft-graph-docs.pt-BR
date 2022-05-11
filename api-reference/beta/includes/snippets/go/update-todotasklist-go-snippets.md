---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b563ff4b2236881474f303f649be457caf5d09b0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Vacation Plan"
requestBody.SetDisplayName(&displayName)
todoTaskListId := "todoTaskList-id"
graphClient.Me().Todo().ListsById(&todoTaskListId).Patch(requestBody)


```