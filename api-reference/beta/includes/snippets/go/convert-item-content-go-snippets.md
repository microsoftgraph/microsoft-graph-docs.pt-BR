---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4f3648ad167ca76c19655f216365902ff99cae3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ContentRequestBuilderGetQueryParameters{
    Format: "%7Bformat%7D",
}
options := &msgraphsdk.ContentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Content().GetWithRequestConfigurationAndResponseHandler(options, nil)


```