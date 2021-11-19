---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 972bad3a5b2cde18d3f0661e4c6056fe59ded762
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104015"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
options := &msgraphsdk.FavoriteRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().Favorite().Post(options)


```