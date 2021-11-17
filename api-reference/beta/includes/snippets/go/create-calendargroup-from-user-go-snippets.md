---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16105aea14cd908afbe6024337338b2830db7c4e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendarGroup()
name := "Personal events"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CalendarGroups().Post(options)


```