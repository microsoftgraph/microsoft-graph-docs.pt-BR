---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1e3be7e1a3f037657d51fa45d048368b140f6b9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287073"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ReprovisionCloudPc().Post(nil)


```