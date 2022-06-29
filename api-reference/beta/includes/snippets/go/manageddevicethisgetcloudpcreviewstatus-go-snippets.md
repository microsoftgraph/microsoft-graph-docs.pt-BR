---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1338a4fdf66161c4c6933d09bdc23ac80cac09fb
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694551"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceId := "managedDevice-id"
result, err := graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).GetCloudPcReviewStatus()(managedDevice-id).Get()


```