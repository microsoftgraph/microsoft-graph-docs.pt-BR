---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 239078992408ca0a32edad8105ade23aa43a37ae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323183"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Untrusted IP named location"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "isTrusted": false,
    "ipRanges":  []Object {
    }
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Post(requestBody)


```