---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa7dae8bb517cf94bcc5e14201571343b9ac07f1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323482"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsedRequestBuilderGetQueryParameters{
    Orderby: "LastUsed/LastAccessedDateTime%20desc",
}
options := &msgraphsdk.UsedRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Insights().Used().GetWithRequestConfigurationAndResponseHandler(options, nil)


```