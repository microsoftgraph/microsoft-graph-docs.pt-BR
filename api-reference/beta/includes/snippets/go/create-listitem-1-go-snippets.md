---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5b83b31913b9e9c8fdc33da2bdcdffcaafbd874
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324868"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewListItem()
fields := msgraphsdk.NewFieldValueSet()
requestBody.SetFields(fields)
fields.SetAdditionalData(map[string]interface{}{
    "Title": "Widget",
    "Color": "Purple",
    "Weight": ,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Items().Post(requestBody)


```