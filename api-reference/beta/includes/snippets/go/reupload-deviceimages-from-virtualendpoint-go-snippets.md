---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b00666be93636f88759aa470465e415d3889185f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcDeviceImageId := "cloudPcDeviceImage-id"
graphClient.DeviceManagement().VirtualEndpoint().DeviceImagesById(&cloudPcDeviceImageId).Reupload().Post(nil)


```