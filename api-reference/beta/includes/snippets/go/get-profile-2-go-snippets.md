---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 579a1f420a25bcb88f28f7ac5e11903056e8307d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325599"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ProfileRequestBuilderGetQueryParameters{
    Expand: "names($select=first,last),skills($select=displayName)",
}
options := &msgraphsdk.ProfileRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Profile().GetWithRequestConfigurationAndResponseHandler(options, nil)


```