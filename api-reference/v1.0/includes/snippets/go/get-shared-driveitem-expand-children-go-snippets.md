---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2020380732e24768152c8df1cc3f6d3400e74e1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322743"
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
sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).DriveItem().GetWithRequestConfigurationAndResponseHandler(options, nil)


```