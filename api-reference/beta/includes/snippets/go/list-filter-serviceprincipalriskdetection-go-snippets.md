---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52d8ebd37fe1ae8152e6e791eaa26e61dfe549e4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325377"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters{
    Filter: "riskEventType%20eq%20'investigationsThreatIntelligence'%20or%20riskLevel%20eq%20'medium'",
}
options := &msgraphsdk.ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityProtection().ServicePrincipalRiskDetections().GetWithRequestConfigurationAndResponseHandler(options, nil)


```