---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27f5579a84b2e1b5b59bfd27746ba3600cd9ad89
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323103"
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
result, err := graphClient.Me().Profile().Websites().Post(requestBody)


```