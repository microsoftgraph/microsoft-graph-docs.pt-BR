---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6479d1586498a4be346a3640fc84daa6fd3042f8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceId := "managedDevice-id"
result, err := graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).GetCloudPcRemoteActionResults()(managedDevice-id).Get()


```