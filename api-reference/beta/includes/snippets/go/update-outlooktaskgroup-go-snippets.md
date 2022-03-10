---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcf684ba3e28579bc1cbab1e10f3f2bc778b4cd1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411012"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskGroup()
name := "Personal Tasks"
requestBody.SetName(&name)
options := &msgraphsdk.OutlookTaskGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookTaskGroupId := "outlookTaskGroup-id"
result, err := graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).Patch(options)


```