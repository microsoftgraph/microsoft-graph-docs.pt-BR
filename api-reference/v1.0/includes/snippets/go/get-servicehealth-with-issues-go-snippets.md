---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26608dd22192a72a08b7d7e45e7a417f69c1a154
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServiceHealthRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.ServiceHealthRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```