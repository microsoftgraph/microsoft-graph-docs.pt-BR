---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5adbd7adc33ac36d617a9692cbfa0cc5edd7f2a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324527"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
options := &msgraphsdk.DeltaRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Groups().Delta()().GetWithRequestConfigurationAndResponseHandler(options, nil)


```