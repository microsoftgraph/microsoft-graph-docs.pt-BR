---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c2e0b99a1f7187cd6ffb5d291dccf9dffe46ee6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006449"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewDevice()
accountEnabled := false
requestBody.SetAccountEnabled(&accountEnabled)
options := &msgraphsdk.DeviceRequestBuilderPatchOptions{
    Body: requestBody,
}
deviceId := "device-id"
graphClient.DevicesById(&deviceId).Patch(options)


```