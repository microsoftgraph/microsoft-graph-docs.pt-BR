---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b953e70ed24a6897d9ab583030de42bb14e212d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters{
    Select: "id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse",
}
options := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```