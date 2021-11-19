---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5cb221302ab0c9110dd8c923a124686249543f6c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085677"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetValue( []Alert {
    msgraphsdk.NewAlert(),
    SetAdditionalData(map[string]interface{}{
        "assignedTo": "String",
        "closedDateTime": "String (timestamp)",
        "comments":  []String {
            "String",
        }
        "id": "String (identifier)",
        "tags":  []String {
            "String",
        }
    }
}
options := &msgraphsdk.UpdateAlertsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().Alerts().UpdateAlerts().Post(options)


```