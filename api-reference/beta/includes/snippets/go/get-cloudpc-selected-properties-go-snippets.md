---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c21f4272481107ca54b72f2fe8d0d406484316a2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324948"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPCRequestBuilderGetQueryParameters{
    Select: "id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult",
}
options := &msgraphsdk.CloudPCRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
cloudPCId := "cloudPC-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```