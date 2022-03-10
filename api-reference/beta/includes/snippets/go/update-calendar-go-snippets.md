---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c846cf511bd64986ea162c766851c19d0c5d91f1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410835"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Social events"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Calendar().Patch(options)


```