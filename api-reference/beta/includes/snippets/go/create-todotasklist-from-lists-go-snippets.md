---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4a3c9778b3c93458b8708c0881155c94ccd3323
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Travel items"
requestBody.SetDisplayName(&displayName)
result, err := graphClient.Me().Todo().Lists().Post(requestBody)


```