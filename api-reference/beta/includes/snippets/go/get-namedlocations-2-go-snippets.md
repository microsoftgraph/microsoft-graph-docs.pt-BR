---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3be181e27bbe0717c3b45b160714c7e8848bbcf8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323719"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.NamedLocationsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.ipNamedLocation')",
}
options := &msgraphsdk.NamedLocationsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().GetWithRequestConfigurationAndResponseHandler(options, nil)


```