---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 594e3c1ddeb8ade221f38efcf6d9d906327127d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324864"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDestinationTaskListIdRequestBody()
destinationTaskListId := "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG"
requestBody.SetDestinationTaskListId(&destinationTaskListId)
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).Move(baseTaskList-id, baseTask-id).Post(requestBody)


```