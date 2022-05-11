---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 416c9b97fb3adc97869fdc9468be052c5e2e0f70
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322204"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
graphClient.Teamwork().DevicesById(&teamworkDeviceId).RunDiagnostics(teamworkDevice-id).Post()


```