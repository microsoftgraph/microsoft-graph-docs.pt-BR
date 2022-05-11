---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 789e9c0b69ce962738daa34aadf1deb206f6cb94
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325316"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
graphClient.DevicesById(&deviceId).Delete()


```