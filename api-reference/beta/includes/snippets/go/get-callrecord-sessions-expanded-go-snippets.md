---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9ff6b2095cad8378f0567b5577c7ee728081260
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324738"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SessionsRequestBuilderGetQueryParameters{
    Expand: "segments",
}
options := &msgraphsdk.SessionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).Sessions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```