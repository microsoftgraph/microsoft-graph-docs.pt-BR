---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef27db7e3af60bea16cef68afd0dc497959079c1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324466"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Filter: "Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')",
    Expand: "Extensions($filter=id%20eq%20'Com.Contoso.Referral')",
}
options := &msgraphsdk.MessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Messages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```