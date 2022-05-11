---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc2b12a467e46819fbed8ec9a81a55f415cfd0fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324498"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DevicesRequestBuilderGetQueryParameters{
    Search: "%22displayName:Android%22",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DevicesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Devices().GetWithRequestConfigurationAndResponseHandler(options, nil)


```