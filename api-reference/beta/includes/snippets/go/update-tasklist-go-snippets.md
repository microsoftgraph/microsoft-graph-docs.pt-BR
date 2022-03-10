---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8814d08273d9f779d0fd98f9cec9d2dd236bd66
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410751"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTaskList()
displayName := "Travel Plan"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.BaseTaskListRequestBuilderPatchOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).Patch(options)


```