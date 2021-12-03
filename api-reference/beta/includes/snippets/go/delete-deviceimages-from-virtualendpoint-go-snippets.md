---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d4b2a47fe785ff66868cf271cc6c0fbf8f5eb4b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcDeviceImageId := "cloudPcDeviceImage-id"
graphClient.DeviceManagement().VirtualEndpoint().DeviceImagesById(&cloudPcDeviceImageId).Delete(nil)


```