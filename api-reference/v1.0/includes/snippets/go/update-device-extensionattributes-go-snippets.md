---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18f8afea69d53080791d9cf4ab06bc5e2fcf55e6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322782"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
requestBody.SetAdditionalData(map[string]interface{}{
}
deviceId := "device-id"
graphClient.DevicesById(&deviceId).Patch(requestBody)


```