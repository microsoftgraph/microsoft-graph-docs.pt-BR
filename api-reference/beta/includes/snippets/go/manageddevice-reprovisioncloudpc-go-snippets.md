---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 597159ddb0677c6007d5c2f6e0dd9887644be1e3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ReprovisionCloudPc(managedDevice-id).Post(nil)


```