---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cec51b0d5ac70ee91f4c331abd6480e29c34aede
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RiskDetectionsRequestBuilderGetQueryParameters{
    Filter: "riskEventType%20eq%20'unfamiliarFeatures'%20or%20riskLevel%20eq%20'medium'",
}
options := &msgraphsdk.RiskDetectionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskDetections().Get(options)


```