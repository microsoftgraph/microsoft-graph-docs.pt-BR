---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e6d16007cbc52e6d45a4d6992c7ca55b36b9831
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323483"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewThreatAssessmentRequest()
expectedAssessment := "block"
requestBody.SetExpectedAssessment(&expectedAssessment)
category := "malware"
requestBody.SetCategory(&category)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.fileAssessmentRequest",
    "fileName": "test.txt",
    "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ==",
}
result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Post(requestBody)


```