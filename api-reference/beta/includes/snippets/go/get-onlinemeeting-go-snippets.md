---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa80cf75514ee801e8b5169b92707b02ce9b50c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324126"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnlineMeetingsRequestBuilderGetQueryParameters{
    Filter: "VideoTeleconferenceId%20eq%20'123456789'",
}
options := &msgraphsdk.OnlineMeetingsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Communications().OnlineMeetings().GetWithRequestConfigurationAndResponseHandler(options, nil)


```