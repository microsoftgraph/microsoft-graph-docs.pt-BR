---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da1d124ce0268a51b180924ad516124dfb5a0c5f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location",
}
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.EventsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Me().Events().Get(options)


```