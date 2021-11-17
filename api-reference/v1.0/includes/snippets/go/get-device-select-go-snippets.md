---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 700eee5b088fb14d3a4cb1bf20b30fdde42eccc8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031154"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DeviceRequestBuilderGetQueryParameters{
    Select: "id,extensionAttributes",
}
options := &msgraphsdk.DeviceRequestBuilderGetOptions{
    Q: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Get(options)


```