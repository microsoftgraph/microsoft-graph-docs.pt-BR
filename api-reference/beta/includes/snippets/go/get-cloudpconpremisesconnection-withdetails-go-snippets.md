---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48205f3d0ed4bdd7f6edb29c4c310927765d4a8b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters{
    Select: "id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse",
}
options := &msgraphsdk.CloudPcOnPremisesConnectionRequestBuilderGetOptions{
    Q: requestParameters,
}
cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).Get(options)


```