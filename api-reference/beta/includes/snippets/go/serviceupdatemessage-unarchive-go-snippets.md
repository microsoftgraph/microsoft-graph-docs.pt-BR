---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f08bad9de163b0c0d70a77eddb34c94568372235
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325020"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageIdsRequestBody()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().Unarchive().Post(requestBody)


```