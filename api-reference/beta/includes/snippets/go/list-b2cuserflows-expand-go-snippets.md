---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15cda77642fceceef7b850c6da76f2bd6d8a37f9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325534"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.B2cUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Identity().B2cUserFlows().GetWithRequestConfigurationAndResponseHandler(options, nil)


```