---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43e1aedcb2f4ecfa44bdee58d13304fb7b91e01d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324781"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.NamedLocationsRequestBuilderGetQueryParameters{
    Filter: "microsoft.graph.countryNamedLocation/countriesAndRegions/any(c:%20c%20eq%20'CA')",
}
options := &msgraphsdk.NamedLocationsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().GetWithRequestConfigurationAndResponseHandler(options, nil)


```