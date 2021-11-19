---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3871f6085fc01c62ba91fc230c627d3d66e90e1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091952"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlace()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.room",
    "nickname": "Conf Room",
    "building": "1",
    "label": "100",
    "capacity": ,
    "isWheelChairAccessible": false,
}
options := &msgraphsdk.PlaceRequestBuilderPatchOptions{
    Body: requestBody,
}
placeId := "place-id"
graphClient.PlacesById(&placeId).Patch(options)


```