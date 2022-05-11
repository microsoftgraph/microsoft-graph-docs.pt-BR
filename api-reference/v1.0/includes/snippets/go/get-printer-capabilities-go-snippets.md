---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b7095492db84892a8f2ca9633f84b5d93e0c0a1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrinterRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```