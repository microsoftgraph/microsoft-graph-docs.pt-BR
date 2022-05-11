---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23210d2bd278830741e6363f1d9a3d2d4297535c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RiskDetectionsRequestBuilderGetQueryParameters{
    Filter: "riskEventType%20eq%20'unfamiliarFeatures'%20or%20riskLevel%20eq%20'medium'",
}
options := &msgraphsdk.RiskDetectionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskDetections().GetWithRequestConfigurationAndResponseHandler(options, nil)


```