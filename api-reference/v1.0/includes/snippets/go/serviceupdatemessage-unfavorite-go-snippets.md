---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a63599c12c4709de33f723558963c9e2c6f3e5c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322745"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageIdsRequestBody()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().Unfavorite().Post(requestBody)


```