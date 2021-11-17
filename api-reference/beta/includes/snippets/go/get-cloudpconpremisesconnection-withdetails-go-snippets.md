---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30054c1d6012d5c19498add4904d2d052f567a19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975676"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters{
    Select: "id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse",
}
options := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetOptions{
    Q: requestParameters,
}
cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).Get(options)


```