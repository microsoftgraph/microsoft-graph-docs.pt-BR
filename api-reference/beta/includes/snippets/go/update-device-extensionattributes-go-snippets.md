---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 426add7ef593db27f0be7cbd760bacf305cb021c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
extensionAttributes := msgraphsdk.NewOnPremisesExtensionAttributes()
requestBody.SetExtensionAttributes(extensionAttributes)
extensionAttribute1 := "BYOD-Device"
extensionAttributes.SetExtensionAttribute1(&extensionAttribute1)
deviceId := "device-id"
graphClient.DevicesById(&deviceId).Patch(requestBody)


```