---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 118c7f2e8fbe4cf123e7b64859a37854915fa1be
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322387"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.BundlesRequestBuilderGetQueryParameters{
    Filter: "bundle/album%20ne%20null",
}
options := &msgraphsdk.BundlesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Drive().Bundles().GetWithRequestConfigurationAndResponseHandler(options, nil)


```