---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9173c44f9c35b6a816ad121940c66544bed52ec7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323602"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTaskList()
displayName := "Shopping list"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.taskList",
}
result, err := graphClient.Me().Tasks().Lists().Post(requestBody)


```