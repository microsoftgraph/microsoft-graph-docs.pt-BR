---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8527efbe865e49976fa64148b7d0314a7f04c55
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322957"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DriveItemRequestBuilderGetQueryParameters{
    Expand: "children",
}
options := &msgraphsdk.DriveItemRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
driveItemId := "driveItem-id"
result, err := graphClient.Drive().ItemsById(&driveItemId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```