---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93b0ad297be4b12bc90aa453cb2d5718030825ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028453"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewThreatAssessmentRequest()
expectedAssessment := "block"
requestBody.SetExpectedAssessment(&expectedAssessment)
category := "phishing"
requestBody.SetCategory(&category)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.urlAssessmentRequest",
    "url": "http://test.com",
}
options := &msgraphsdk.ThreatAssessmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Post(options)


```