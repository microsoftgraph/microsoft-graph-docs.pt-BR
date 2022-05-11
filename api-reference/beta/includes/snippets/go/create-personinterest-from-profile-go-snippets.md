---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9271bf14f628d2120c406441286626ff8858ce12
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322996"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
description := "World's greatest football club"
requestBody.SetDescription(&description)
displayName := "Chelsea FC"
requestBody.SetDisplayName(&displayName)
webUrl := "https://www.chelseafc.com"
requestBody.SetWebUrl(&webUrl)
result, err := graphClient.Me().Profile().Interests().Post(requestBody)


```