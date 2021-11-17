---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 770aac0c7da98f12139bd8d0903085fc21359b90
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookTaskGroup()
name := "Leisure tasks"
requestBody.SetName(&name)
options := &msgraphsdk.TaskGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().TaskGroups().Post(options)


```