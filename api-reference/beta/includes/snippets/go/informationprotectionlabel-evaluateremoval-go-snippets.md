---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5649f5c5836cf3de377d918e4230bfa8e841fd7f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
contentInfo := msgraphsdk.NewContentInfo()
requestBody.SetContentInfo(contentInfo)
format := "default"
contentInfo.SetFormat(&format)
contentInfo.SetIdentifier(nil)
state := "rest"
contentInfo.SetState(&state)
contentInfo.SetMetadata( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled"
    SetName(&name)
value := "True"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method"
    SetName(&name)
value := "Standard"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate"
    SetName(&name)
value := "1/1/0001 12:00:00 AM"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId"
    SetName(&name)
value := "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name"
    SetName(&name)
value := "General"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits"
    SetName(&name)
value := "0"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
    SetName(&name)
value := "00000000-0000-0000-0000-000000000000"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
}
contentInfo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "state@odata.type": "#microsoft.graph.contentState",
    "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
}
downgradeJustification := msgraphsdk.NewDowngradeJustification()
requestBody.SetDowngradeJustification(downgradeJustification)
justificationMessage := "The information has been declassified."
downgradeJustification.SetJustificationMessage(&justificationMessage)
isDowngradeJustified := true
downgradeJustification.SetIsDowngradeJustified(&isDowngradeJustified)
headers := map[string]string{
    "User-Agent": "ContosoLOBApp/1.0"
}
options := &msgraphsdk.EvaluateRemovalRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.InformationProtection().Policy().Labels().EvaluateRemoval().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```