---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 584d52d6aa4fb1cf72157dad4d21dba6176f9fe1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100188"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonWebsite()
requestBody.SetCategories( []String {
    "football",
}
displayName := "Lyn Damer"
requestBody.SetDisplayName(&displayName)
webUrl := "www.lyndamer.no"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.WebsitesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Websites().Post(options)


```