---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62aa91541582e617c8a2fc1e9c53b472964c2d58
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020492"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
options := &msgraphsdk.MarkReadRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().MarkRead().Post(options)


```