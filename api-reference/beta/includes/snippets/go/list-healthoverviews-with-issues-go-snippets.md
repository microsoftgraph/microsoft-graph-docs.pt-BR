---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4261125edc666bf8eeb004c431a8315da6d304cc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.HealthOverviewsRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.HealthOverviewsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().GetWithRequestConfigurationAndResponseHandler(options, nil)


```