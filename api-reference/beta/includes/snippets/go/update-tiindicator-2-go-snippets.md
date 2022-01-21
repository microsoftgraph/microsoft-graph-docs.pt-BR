---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96bf5e3201f7dd05143a388aec2513addc29d66c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115544"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTiIndicator()
additionalInformation := "additionalInformation-after-update"
requestBody.SetAdditionalInformation(&additionalInformation)
confidence := int32(42)
requestBody.SetConfidence(&confidence)
description := "description-after-update"
requestBody.SetDescription(&description)
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TiIndicatorRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
tiIndicatorId := "tiIndicator-id"
graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(options)


```