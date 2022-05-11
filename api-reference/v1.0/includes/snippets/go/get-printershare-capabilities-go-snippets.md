---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34e0c6fc6b43f5a1b4f65381f5ac983b3d609b53
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322853"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrinterShareRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterShareRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```